
---
title: "ActionGroup"
block_external_search_index: true
---

Manages an Action Group within Azure Monitor.

> This content is derived from https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/monitor_action_group.html.markdown.



## Create a ActionGroup Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/azure/monitoring/#ActionGroup">ActionGroup</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/azure/monitoring/#ActionGroupArgs">ActionGroupArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">ActionGroup</span><span class="p">(resource_name, opts=None, </span>arm_role_receivers=None<span class="p">, </span>automation_runbook_receivers=None<span class="p">, </span>azure_app_push_receivers=None<span class="p">, </span>azure_function_receivers=None<span class="p">, </span>email_receivers=None<span class="p">, </span>enabled=None<span class="p">, </span>itsm_receivers=None<span class="p">, </span>logic_app_receivers=None<span class="p">, </span>name=None<span class="p">, </span>resource_group_name=None<span class="p">, </span>short_name=None<span class="p">, </span>sms_receivers=None<span class="p">, </span>tags=None<span class="p">, </span>voice_receivers=None<span class="p">, </span>webhook_receivers=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewActionGroup<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupArgs">ActionGroupArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroup">ActionGroup</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Azure/Pulumi.Azure.Monitoring.ActionGroup.html">ActionGroup</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Azure/Pulumi.Azure.Monitoring.ActionGroupArgs.html">ActionGroupArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">List&lt;Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">List&lt;Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">List&lt;Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">List&lt;Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">List&lt;Action<wbr>Group<wbr>Email<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">List&lt;Action<wbr>Group<wbr>Itsm<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">List&lt;Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">List&lt;Action<wbr>Group<wbr>Sms<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, string>?</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">List&lt;Action<wbr>Group<wbr>Voice<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">List&lt;Action<wbr>Group<wbr>Webhook<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">[]Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">[]Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">[]Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">[]Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">[]Action<wbr>Group<wbr>Email<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">[]Action<wbr>Group<wbr>Itsm<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">[]Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">[]Action<wbr>Group<wbr>Sms<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">[]Action<wbr>Group<wbr>Voice<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">[]Action<wbr>Group<wbr>Webhook<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">Action<wbr>Group<wbr>Email<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">Action<wbr>Group<wbr>Itsm<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">Action<wbr>Group<wbr>Sms<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}?</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">Action<wbr>Group<wbr>Voice<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">Action<wbr>Group<wbr>Webhook<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>arm_<wbr>role_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">List[Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>automation_<wbr>runbook_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">List[Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure_<wbr>app_<wbr>push_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">List[Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure_<wbr>function_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">List[Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">List[Action<wbr>Group<wbr>Email<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>itsm_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">List[Action<wbr>Group<wbr>Itsm<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>logic_<wbr>app_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">List[Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>resource_<wbr>group_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>short_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">List[Action<wbr>Group<wbr>Sms<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, str]</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>voice_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">List[Action<wbr>Group<wbr>Voice<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>webhook_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">List[Action<wbr>Group<wbr>Webhook<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## ActionGroup Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">List&lt;Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">List&lt;Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">List&lt;Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">List&lt;Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">List&lt;Action<wbr>Group<wbr>Email<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">List&lt;Action<wbr>Group<wbr>Itsm<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">List&lt;Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">List&lt;Action<wbr>Group<wbr>Sms<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, string>?</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">List&lt;Action<wbr>Group<wbr>Voice<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">List&lt;Action<wbr>Group<wbr>Webhook<wbr>Receiver&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">[]Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">[]Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">[]Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">[]Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">[]Action<wbr>Group<wbr>Email<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">[]Action<wbr>Group<wbr>Itsm<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">[]Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">[]Action<wbr>Group<wbr>Sms<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">[]Action<wbr>Group<wbr>Voice<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">[]Action<wbr>Group<wbr>Webhook<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">Action<wbr>Group<wbr>Email<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">Action<wbr>Group<wbr>Itsm<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">Action<wbr>Group<wbr>Sms<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}?</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">Action<wbr>Group<wbr>Voice<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">Action<wbr>Group<wbr>Webhook<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>arm_<wbr>role_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">List[Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>automation_<wbr>runbook_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">List[Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>azure_<wbr>app_<wbr>push_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">List[Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>azure_<wbr>function_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">List[Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>email_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">List[Action<wbr>Group<wbr>Email<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>itsm_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">List[Action<wbr>Group<wbr>Itsm<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>logic_<wbr>app_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">List[Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>resource_<wbr>group_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>short_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>sms_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">List[Action<wbr>Group<wbr>Sms<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, str]</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>voice_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">List[Action<wbr>Group<wbr>Voice<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>webhook_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">List[Action<wbr>Group<wbr>Webhook<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing ActionGroup Resource

Get an existing ActionGroup resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/azure/monitoring/#ActionGroupState">ActionGroupState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/azure/monitoring/#ActionGroup">ActionGroup</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>arm_role_receivers=None<span class="p">, </span>automation_runbook_receivers=None<span class="p">, </span>azure_app_push_receivers=None<span class="p">, </span>azure_function_receivers=None<span class="p">, </span>email_receivers=None<span class="p">, </span>enabled=None<span class="p">, </span>itsm_receivers=None<span class="p">, </span>logic_app_receivers=None<span class="p">, </span>name=None<span class="p">, </span>resource_group_name=None<span class="p">, </span>short_name=None<span class="p">, </span>sms_receivers=None<span class="p">, </span>tags=None<span class="p">, </span>voice_receivers=None<span class="p">, </span>webhook_receivers=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetActionGroup<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupState">ActionGroupState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroup">ActionGroup</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Azure/Pulumi.Azure.Monitoring.ActionGroup.html">ActionGroup</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Azure/Pulumi.Azure.Monitoring.ActionGroupState.html">ActionGroupState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">List&lt;Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">List&lt;Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">List&lt;Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">List&lt;Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">List&lt;Action<wbr>Group<wbr>Email<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">List&lt;Action<wbr>Group<wbr>Itsm<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">List&lt;Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">List&lt;Action<wbr>Group<wbr>Sms<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, string>?</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">List&lt;Action<wbr>Group<wbr>Voice<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">List&lt;Action<wbr>Group<wbr>Webhook<wbr>Receiver<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">[]Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">[]Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">[]Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">[]Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">[]Action<wbr>Group<wbr>Email<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">[]Action<wbr>Group<wbr>Itsm<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">[]Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">[]Action<wbr>Group<wbr>Sms<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">[]Action<wbr>Group<wbr>Voice<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">[]Action<wbr>Group<wbr>Webhook<wbr>Receiver</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>arm<wbr>Role<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>automation<wbr>Runbook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure<wbr>App<wbr>Push<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure<wbr>Function<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">Action<wbr>Group<wbr>Email<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>itsm<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">Action<wbr>Group<wbr>Itsm<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>logic<wbr>App<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>resource<wbr>Group<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>short<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">Action<wbr>Group<wbr>Sms<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}?</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>voice<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">Action<wbr>Group<wbr>Voice<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>webhook<wbr>Receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">Action<wbr>Group<wbr>Webhook<wbr>Receiver[]?</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>arm_<wbr>role_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouparmrolereceiver">List[Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `arm_role_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>automation_<wbr>runbook_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupautomationrunbookreceiver">List[Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `automation_runbook_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure_<wbr>app_<wbr>push_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazureapppushreceiver">List[Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_app_push_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>azure_<wbr>function_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupazurefunctionreceiver">List[Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `azure_function_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>email_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupemailreceiver">List[Action<wbr>Group<wbr>Email<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `email_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this action group is enabled. If an action group is not enabled, then none of its receivers will receive communications. Defaults to `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>itsm_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupitsmreceiver">List[Action<wbr>Group<wbr>Itsm<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `itsm_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>logic_<wbr>app_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongrouplogicappreceiver">List[Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `logic_app_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Action Group. Changing this forces a new resource to be created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>resource_<wbr>group_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group in which to create the Action Group instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>short_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The short name of the action group. This will be used in SMS messages.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sms_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupsmsreceiver">List[Action<wbr>Group<wbr>Sms<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `sms_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, str]</span>
    </dt>
    <dd>{{% md %}}A mapping of tags to assign to the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>voice_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupvoicereceiver">List[Action<wbr>Group<wbr>Voice<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `voice_receiver` blocks as defined below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>webhook_<wbr>receivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#actiongroupwebhookreceiver">List[Action<wbr>Group<wbr>Webhook<wbr>Receiver]</a></span>
    </dt>
    <dd>{{% md %}}One or more `webhook_receiver` blocks as defined below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Action<wbr>Group<wbr>Arm<wbr>Role<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupArmRoleReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupArmRoleReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupArmRoleReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupArmRoleReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the ARM role receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Role<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The arm role id.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the ARM role receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Role<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The arm role id.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the ARM role receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>role<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The arm role id.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the ARM role receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>role<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The arm role id.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Automation<wbr>Runbook<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupAutomationRunbookReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupAutomationRunbookReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupAutomationRunbookReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupAutomationRunbookReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Automation<wbr>Account<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The automation account ID which holds this runbook and authenticates to Azure resources.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Is<wbr>Global<wbr>Runbook</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether this instance is global runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the automation runbook receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Runbook<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name for this runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Service<wbr>Uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Webhook<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource id for webhook linked to this runbook.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Automation<wbr>Account<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The automation account ID which holds this runbook and authenticates to Azure resources.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Is<wbr>Global<wbr>Runbook</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether this instance is global runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the automation runbook receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Runbook<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name for this runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Service<wbr>Uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Webhook<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource id for webhook linked to this runbook.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>automation<wbr>Account<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The automation account ID which holds this runbook and authenticates to Azure resources.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>is<wbr>Global<wbr>Runbook</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Indicates whether this instance is global runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the automation runbook receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>runbook<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name for this runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>service<wbr>Uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>webhook<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource id for webhook linked to this runbook.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>automation<wbr>Account<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The automation account ID which holds this runbook and authenticates to Azure resources.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>is<wbr>Global<wbr>Runbook</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicates whether this instance is global runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the automation runbook receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>runbook_<wbr>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name for this runbook.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>service_<wbr>uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>webhook<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The resource id for webhook linked to this runbook.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Azure<wbr>App<wbr>Push<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupAzureAppPushReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupAzureAppPushReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupAzureAppPushReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupAzureAppPushReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Email<wbr>Address</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The email address of the user signed into the mobile app who will receive push notifications from this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Azure app push receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Email<wbr>Address</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The email address of the user signed into the mobile app who will receive push notifications from this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Azure app push receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>email<wbr>Address</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The email address of the user signed into the mobile app who will receive push notifications from this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Azure app push receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>email_<wbr>address</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The email address of the user signed into the mobile app who will receive push notifications from this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Azure app push receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Azure<wbr>Function<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupAzureFunctionReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupAzureFunctionReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupAzureFunctionReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupAzureFunctionReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Function<wbr>App<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Function<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The function name in the function app.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Http<wbr>Trigger<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The http trigger url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Azure Function receiver.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Function<wbr>App<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Function<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The function name in the function app.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Http<wbr>Trigger<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The http trigger url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Azure Function receiver.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>function<wbr>App<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>function<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The function name in the function app.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>http<wbr>Trigger<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The http trigger url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Azure Function receiver.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>function<wbr>App<wbr>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>function<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The function name in the function app.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>http<wbr>Trigger<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The http trigger url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Azure Function receiver.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Email<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupEmailReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupEmailReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupEmailReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupEmailReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Email<wbr>Address</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The email address of this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the email receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Email<wbr>Address</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The email address of this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the email receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>email<wbr>Address</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The email address of this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the email receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>email_<wbr>address</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The email address of this receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the email receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Itsm<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupItsmReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupItsmReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupItsmReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupItsmReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Connection<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The unique connection identifier of the ITSM connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the ITSM receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region of the workspace.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ticket<wbr>Configuration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A JSON blob for the configurations of the ITSM action. CreateMultipleWorkItems option will be part of this blob as well.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Workspace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Azure Log Analytics workspace ID where this connection is defined.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Connection<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The unique connection identifier of the ITSM connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the ITSM receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region of the workspace.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ticket<wbr>Configuration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A JSON blob for the configurations of the ITSM action. CreateMultipleWorkItems option will be part of this blob as well.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Workspace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Azure Log Analytics workspace ID where this connection is defined.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>connection<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The unique connection identifier of the ITSM connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the ITSM receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region of the workspace.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ticket<wbr>Configuration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A JSON blob for the configurations of the ITSM action. CreateMultipleWorkItems option will be part of this blob as well.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>workspace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Azure Log Analytics workspace ID where this connection is defined.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>connection<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The unique connection identifier of the ITSM connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the ITSM receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region of the workspace.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ticket<wbr>Configuration</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A JSON blob for the configurations of the ITSM action. CreateMultipleWorkItems option will be part of this blob as well.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>workspace_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Azure Log Analytics workspace ID where this connection is defined.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Logic<wbr>App<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupLogicAppReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupLogicAppReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupLogicAppReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupLogicAppReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Callback<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The callback url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the logic app receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Azure resource ID of the logic app.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Callback<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The callback url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the logic app receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Azure resource ID of the logic app.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>callback<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The callback url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the logic app receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>resource<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Azure resource ID of the logic app.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>callback<wbr>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The callback url where http request sent to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the logic app receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>resource_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Azure resource ID of the logic app.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Sms<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupSmsReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupSmsReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupSmsReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupSmsReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The country code of the SMS receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the SMS receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The phone number of the SMS receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The country code of the SMS receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the SMS receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The phone number of the SMS receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The country code of the SMS receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the SMS receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The phone number of the SMS receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The country code of the SMS receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the SMS receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The phone number of the SMS receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Voice<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupVoiceReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupVoiceReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupVoiceReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupVoiceReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The country code of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The phone number of the voice receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The country code of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The phone number of the voice receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The country code of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The phone number of the voice receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>country<wbr>Code</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The country code of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the voice receiver.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>phone<wbr>Number</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The phone number of the voice receiver.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Action<wbr>Group<wbr>Webhook<wbr>Receiver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/input/#ActionGroupWebhookReceiver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/azure/types/output/#ActionGroupWebhookReceiver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupWebhookReceiverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/go/azure/monitoring?tab=doc#ActionGroupWebhookReceiverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the webhook receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Service<wbr>Uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the webhook receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Service<wbr>Uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the webhook receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>service<wbr>Uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the webhook receiver. Names must be unique (case-insensitive) across all receivers within an action group.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>service_<wbr>uri</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The URI where webhooks should be sent.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>use<wbr>Common<wbr>Alert<wbr>Schema</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enables or disables the common alert schema.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure">https://github.com/pulumi/pulumi-azure</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd></dl>