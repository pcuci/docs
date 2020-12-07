---
title: "Importing Infrastructure"
meta_desc: Learn how to import existing cloud infrastructure into Pulumi no matter how it was provisioned.
menu:
  userguides:
    parent: adopting
    weight: 1
---

Most infrastructure projects require working with existing cloud resources, either by building on top of existing
resources or adopting existing resources under management with a new and more robust infrastructure provisioning solution.

No matter how you've provisioned these resources &mdash; manually in your cloud provider's console or CLI, using an
infrastructure as code tool like Terraform or AWS CloudFormation &mdash; Pulumi enables you to adopt and manage your resources.

<!--more-->

When working with existing resources, there are two primary scenarios:

* You need to reference existing resources to use as inputs to new resources in Pulumi
* You need to adopt existing resources under management so they can be managed by Pulumi

For the first situation, consult [the user guide index]({{< relref "/docs/guides/adopting#coexistence" >}}). For the
second, let's now see how to adopt existing resources.

## Adopting Existing Resources

To adopt existing resources so that Pulumi is able to manage subsequent updates to them, Pulumi offers the
[`import`]({{< relref "/docs/reference/cli/pulumi_import" >}}) cli command option. This option request that a resource
defined in your Pulumi program adopts an existing resource in the cloud provider instead of creating a new one as would
normally occur.

This example imports an existing AWS S3 bucket with name `company-infra-logs`:

```bash
pulumi import aws:s3/bucket:Bucket infra-logs company-infra-logs
```

```
     Type                 Name             Plan
 +   pulumi:pulumi:Stack  import-post-dev  create
 =   └─ aws:s3:Bucket     infra-logs       import

Resources:
    + 1 to create
    = 1 to import
    2 changes
```

Pulumi will perform the import of the S3 bucket and it will generate the code required for the user to add to their
application.

{{< chooser language "typescript,python,csharp,go" >}}

{{< choosable language typescript >}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const demo = new aws.s3.Bucket("infra-logs", {
    acl: "private",
    bucket: "company-infra-logs",
    forceDestroy: false,
}, {
    protect: true,
});
```

{{< /choosable >}}
{{< choosable language python >}}

```python
import pulumi
import pulumi_aws as aws

demo = aws.s3.Bucket("infra-logs",
    acl="private",
    bucket="company-infra-logs",
    force_destroy=False,
    opts=ResourceOptions(protect=True))
```

{{< /choosable >}}
{{< choosable language go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-aws/sdk/v3/go/aws/s3"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := s3.NewBucket(ctx, "infra-logs", &s3.BucketArgs{
			Acl:          pulumi.String("private"),
			Bucket:       pulumi.String("company-infra-logs"),
			ForceDestroy: pulumi.Bool(false),
		}, pulumi.Protect(true))
		if err != nil {
			return err
		}
		return nil
	})
}
```

{{< /choosable >}}
{{< choosable language csharp >}}

```csharp
using Pulumi;
using Aws = Pulumi.Aws;

class MyStack : Stack
{
    public MyStack()
    {
        var demo = new Aws.S3.Bucket("infra-logs", new Aws.S3.BucketArgs
        {
            Acl = "private",
            Bucket = "company-infra-logs",
            ForceDestroy = false,
        }, new CustomResourceOptions
        {
            Protect = true,
        });
    }

}
```

{{< /choosable >}}
{{< /chooser >}}

> Your Pulumi stack must be configured correctly---e.g., in this case, the correct AWS region---otherwise the resource will not be found.

After successfully importing a resource, you can run `pulumi up`, and all subsequent operations will behave as though Pulumi provisioned
the resource from the outset. When Pulumi performs an import, the resource is added to the Pulumi [state](https://www.pulumi.com/docs/intro/concepts/state/#state),
it is marked as a [protected](https://www.pulumi.com/docs/intro/concepts/programming-model/#protect) resource (by default),
and it will emit the generated code that the user can add to their program before running a `pulumi up`. The resources are
marked as protected to ensure that imported infrastructure is not accidentally deleted if the user forgets to include
the code for the resource in their program before doing a deployment.

### Bulk Import Operation

Should a user need to import multiple resources to be managed by Pulumi, the CLI `import command` can handle this
scenario for us. This is helpful when using the pulumi import command as part of scripting larger bulk imports of
cloud resource:

```json
{
	"resources": [{
			"type": "aws:ec2/vpc:Vpc",
			"name": "application-vpc",
			"id": "vpc-0ad77710973388316"
		},
		{
			"type": "aws:ec2/subnet:Subnet",
			"name": "public-1",
			"id": "subnet-0fb5fdff92b9e5a3b"
		},
		{
			"type": "aws:ec2/subnet:Subnet",
			"name": "private-1",
			"id": "subnet-0a39d25dd9f7b7808"
		}
	]
}
```

We can then run the command:

```bash
pulumi import -f resources.json
```

We can then see Pulumi will generate all of the resource code for us as follows:

{{< chooser language "typescript,python,csharp,go" >}}

{{< choosable language typescript >}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const application_vpc = new aws.ec2.Vpc("application-vpc", {
    assignGeneratedIpv6CidrBlock: false,
    cidrBlock: "172.16.0.0/16",
    enableDnsSupport: true,
    instanceTenancy: "default",
    tags: {
        Name: "pulumi-vpc",
        Owner: "pulumi",
        Project: "pulumi-k8s-aws-cluster",
    },
}, {
    protect: true,
});
const public_1 = new aws.ec2.Subnet("public-1", {
    assignIpv6AddressOnCreation: false,
    cidrBlock: "172.16.32.0/19",
    mapPublicIpOnLaunch: true,
    tags: {
        Name: "pulumi-vpc-public-1",
        Owner: "pulumi",
        Project: "pulumi-k8s-aws-cluster",
        "kubernetes.io/role/elb": "1",
        type: "public",
    },
    vpcId: "vpc-0ad77710973388316",
}, {
    protect: true,
});
const private_1 = new aws.ec2.Subnet("private-1", {
    assignIpv6AddressOnCreation: false,
    cidrBlock: "172.16.160.0/19",
    mapPublicIpOnLaunch: false,
    tags: {
        Name: "pulumi-vpc-private-1",
        Owner: "pulumi",
        Project: "pulumi-k8s-aws-cluster",
        "kubernetes.io/role/internal-elb": "1",
        type: "private",
    },
    vpcId: "vpc-0ad77710973388316",
}, {
    protect: true,
});
```

{{< /choosable >}}
{{< choosable language python >}}

```python
import pulumi
import pulumi_aws as aws

application_vpc = aws.ec2.Vpc("application-vpc",
    assign_generated_ipv6_cidr_block=False,
    cidr_block="172.16.0.0/16",
    enable_dns_support=True,
    instance_tenancy="default",
    tags={
        "Name": "pulumi-vpc",
        "Owner": "pulumi",
        "Project": "pulumi-k8s-aws-cluster",
    },
    opts=ResourceOptions(protect=True))
public_1 = aws.ec2.Subnet("public-1",
    assign_ipv6_address_on_creation=False,
    cidr_block="172.16.32.0/19",
    map_public_ip_on_launch=True,
    tags={
        "Name": "pulumi-vpc-public-1",
        "Owner": "pulumi",
        "Project": "pulumi-k8s-aws-cluster",
        "kubernetes.io/role/elb": "1",
        "type": "public",
    },
    vpc_id="vpc-0ad77710973388316",
    opts=ResourceOptions(protect=True))
private_1 = aws.ec2.Subnet("private-1",
    assign_ipv6_address_on_creation=False,
    cidr_block="172.16.160.0/19",
    map_public_ip_on_launch=False,
    tags={
        "Name": "pulumi-vpc-private-1",
        "Owner": "pulumi",
        "Project": "pulumi-k8s-aws-cluster",
        "kubernetes.io/role/internal-elb": "1",
        "type": "private",
    },
    vpc_id="vpc-0ad77710973388316",
    opts=ResourceOptions(protect=True))
```

{{< /choosable >}}
{{< choosable language go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-aws/sdk/v3/go/aws/ec2"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := ec2.NewVpc(ctx, "application_vpc", &ec2.VpcArgs{
			AssignGeneratedIpv6CidrBlock: pulumi.Bool(false),
			CidrBlock:                    pulumi.String("172.16.0.0/16"),
			EnableDnsSupport:             pulumi.Bool(true),
			InstanceTenancy:              pulumi.String("default"),
			Tags: pulumi.StringMap{
				"Name":    pulumi.String("pulumi-vpc"),
				"Owner":   pulumi.String("pulumi"),
				"Project": pulumi.String("pulumi-k8s-aws-cluster"),
			},
		}, pulumi.Protect(true))
		if err != nil {
			return err
		}
		_, err = ec2.NewSubnet(ctx, "public_1", &ec2.SubnetArgs{
			AssignIpv6AddressOnCreation: pulumi.Bool(false),
			CidrBlock:                   pulumi.String("172.16.32.0/19"),
			MapPublicIpOnLaunch:         pulumi.Bool(true),
			Tags: pulumi.StringMap{
				"Name":                   pulumi.String("pulumi-vpc-public-1"),
				"Owner":                  pulumi.String("pulumi"),
				"Project":                pulumi.String("pulumi-k8s-aws-cluster"),
				"kubernetes.io/role/elb": pulumi.String("1"),
				"type":                   pulumi.String("public"),
			},
			VpcId: pulumi.String("vpc-0ad77710973388316"),
		}, pulumi.Protect(true))
		if err != nil {
			return err
		}
		_, err = ec2.NewSubnet(ctx, "private_1", &ec2.SubnetArgs{
			AssignIpv6AddressOnCreation: pulumi.Bool(false),
			CidrBlock:                   pulumi.String("172.16.160.0/19"),
			MapPublicIpOnLaunch:         pulumi.Bool(false),
			Tags: pulumi.StringMap{
				"Name":                            pulumi.String("pulumi-vpc-private-1"),
				"Owner":                           pulumi.String("pulumi"),
				"Project":                         pulumi.String("pulumi-k8s-aws-cluster"),
				"kubernetes.io/role/internal-elb": pulumi.String("1"),
				"type":                            pulumi.String("private"),
			},
			VpcId: pulumi.String("vpc-0ad77710973388316"),
		}, pulumi.Protect(true))
		if err != nil {
			return err
		}
		return nil
	})
}
```

{{< /choosable >}}
{{< choosable language csharp >}}

```csharp
using Pulumi;
using Aws = Pulumi.Aws;

class MyStack : Stack
{
    public MyStack()
    {
        var application_vpc = new Aws.Ec2.Vpc("application-vpc", new Aws.Ec2.VpcArgs
        {
            AssignGeneratedIpv6CidrBlock = false,
            CidrBlock = "172.16.0.0/16",
            EnableDnsSupport = true,
            InstanceTenancy = "default",
            Tags =
            {
                { "Name", "pulumi-vpc" },
                { "Owner", "pulumi" },
                { "Project", "pulumi-k8s-aws-cluster" },
            },
        }, new CustomResourceOptions
        {
            Protect = true,
        });
        var public_1 = new Aws.Ec2.Subnet("public-1", new Aws.Ec2.SubnetArgs
        {
            AssignIpv6AddressOnCreation = false,
            CidrBlock = "172.16.32.0/19",
            MapPublicIpOnLaunch = true,
            Tags =
            {
                { "Name", "pulumi-vpc-public-1" },
                { "Owner", "pulumi" },
                { "Project", "pulumi-k8s-aws-cluster" },
                { "kubernetes.io/role/elb", "1" },
                { "type", "public" },
            },
            VpcId = "vpc-0ad77710973388316",
        }, new CustomResourceOptions
        {
            Protect = true,
        });
        var private_1 = new Aws.Ec2.Subnet("private-1", new Aws.Ec2.SubnetArgs
        {
            AssignIpv6AddressOnCreation = false,
            CidrBlock = "172.16.160.0/19",
            MapPublicIpOnLaunch = false,
            Tags =
            {
                { "Name", "pulumi-vpc-private-1" },
                { "Owner", "pulumi" },
                { "Project", "pulumi-k8s-aws-cluster" },
                { "kubernetes.io/role/internal-elb", "1" },
                { "type", "private" },
            },
            VpcId = "vpc-0ad77710973388316",
        }, new CustomResourceOptions
        {
            Protect = true,
        });
    }

}
```

{{< /choosable >}}
{{< /chooser >}}

Check out the video clip below for a demo.

{{< youtube "6qHVbu8vb4w" >}}
