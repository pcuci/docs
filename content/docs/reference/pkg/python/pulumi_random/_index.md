---
title: Package pulumi_random
title_tag: Package pulumi_random | Python SDK
linktitle: pulumi_random
notitle: true
block_external_search_index: true
---

{{< resource-docs-alert "random" >}}

<div class="section" id="pulumi-random">
<h1>Pulumi Random<a class="headerlink" href="#pulumi-random" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div><p>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-random">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-random/issues">pulumi/pulumi-random repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-random/issues">terraform-providers/terraform-provider-random repo</a>.</p>
</div></blockquote>
<span class="target" id="module-pulumi_random"></span><dl class="py class">
<dt id="pulumi_random.Provider">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">Provider</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.Provider" title="Permalink to this definition">¶</a></dt>
<dd><p>The provider type for the random package. By default, resources use package-wide configuration
settings, however an explicit <code class="docutils literal notranslate"><span class="pre">Provider</span></code> instance may be created and passed during resource
construction to achieve fine-grained programmatic control over provider settings. See the
<a class="reference external" href="https://www.pulumi.com/docs/reference/programming-model/#providers">documentation</a> for more information.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.Provider.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.Provider.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.Provider.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.Provider.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomId">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomId</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">byte_length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">prefix</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomId" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource <code class="docutils literal notranslate"><span class="pre">RandomId</span></code> generates random numbers that are intended to be
used as unique identifiers for other resources.</p>
<p>This resource <em>does</em> use a cryptographic random number generator in order
to minimize the chance of collisions, making the results of this resource
when a 16-byte identifier is requested of equivalent uniqueness to a
type-4 UUID.</p>
<p>This resource can be used in conjunction with resources that have
the <code class="docutils literal notranslate"><span class="pre">create_before_destroy</span></code> lifecycle flag set to avoid conflicts with
unique names during the brief period where both the old and new resources
exist concurrently.</p>
<p>The following example shows how to generate a unique name for an AWS EC2
instance that changes each time a new AMI id is selected.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_aws</span> <span class="k">as</span> <span class="nn">aws</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">server_random_id</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomId</span><span class="p">(</span><span class="s2">&quot;serverRandomId&quot;</span><span class="p">,</span>
    <span class="n">byte_length</span><span class="o">=</span><span class="mi">8</span><span class="p">,</span>
    <span class="n">keepers</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;ami_id&quot;</span><span class="p">:</span> <span class="n">var</span><span class="p">[</span><span class="s2">&quot;ami_id&quot;</span><span class="p">],</span>
    <span class="p">})</span>
<span class="n">server_instance</span> <span class="o">=</span> <span class="n">aws</span><span class="o">.</span><span class="n">ec2</span><span class="o">.</span><span class="n">Instance</span><span class="p">(</span><span class="s2">&quot;serverInstance&quot;</span><span class="p">,</span>
    <span class="n">ami</span><span class="o">=</span><span class="n">server_random_id</span><span class="o">.</span><span class="n">keepers</span><span class="p">[</span><span class="s2">&quot;amiId&quot;</span><span class="p">],</span>
    <span class="n">tags</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;Name&quot;</span><span class="p">:</span> <span class="n">server_random_id</span><span class="o">.</span><span class="n">hex</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="nb">hex</span><span class="p">:</span> <span class="sa">f</span><span class="s2">&quot;web-server </span><span class="si">{</span><span class="nb">hex</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">),</span>
    <span class="p">})</span>
</pre></div>
</div>
<p>Random Ids can be imported using the <code class="docutils literal notranslate"><span class="pre">b64_url</span></code> with an optional <code class="docutils literal notranslate"><span class="pre">prefix</span></code>. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example with no prefix</p>
<div class="highlight-sh notranslate"><div class="highlight"><pre><span></span>   $ pulumi import random:index/randomId:RandomId server p-9hUg

Example with prefix <span class="o">(</span>prefix is separated by a <span class="sb">``</span>,<span class="sb">``</span><span class="se">\ </span><span class="o">)</span>
</pre></div>
</div>
<div class="highlight-sh notranslate"><div class="highlight"><pre><span></span>$ pulumi import random:index/randomId:RandomId server my-prefix-,p-9hUg
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>byte_length</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The number of random bytes to produce. The
minimum value is 1, which produces eight bits of randomness.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>prefix</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Arbitrary string to prefix the output value with. This
string is supplied as-is, meaning it is not guaranteed to be URL-safe or
base64 encoded.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomId.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">b64</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">b64_std</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">b64_url</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">byte_length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dec</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">hex</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">prefix</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_id.RandomId<a class="headerlink" href="#pulumi_random.RandomId.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomId resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>b64_std</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The generated id presented in base64 without additional transformations.</p></li>
<li><p><strong>b64*url</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>The generated id presented in base64, using the URL-friendly character set: case-sensitive letters, digits and the characters <cite>*``and`</cite>-<a href="#id3"><span class="problematic" id="id4">`</span></a>.</p>
</p></li>
<li><p><strong>byte_length</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The number of random bytes to produce. The
minimum value is 1, which produces eight bits of randomness.</p></li>
<li><p><strong>dec</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The generated id presented in non-padded decimal digits.</p></li>
<li><p><strong>hex</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The generated id presented in padded hexadecimal digits. This result will always be twice as long as the requested byte length.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>prefix</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Arbitrary string to prefix the output value with. This
string is supplied as-is, meaning it is not guaranteed to be URL-safe or
base64 encoded.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.b64_std">
<em class="property">property </em><code class="sig-name descname">b64_std</code><a class="headerlink" href="#pulumi_random.RandomId.b64_std" title="Permalink to this definition">¶</a></dt>
<dd><p>The generated id presented in base64 without additional transformations.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.b64_url">
<em class="property">property </em><code class="sig-name descname">b64_url</code><a class="headerlink" href="#pulumi_random.RandomId.b64_url" title="Permalink to this definition">¶</a></dt>
<dd><p>The generated id presented in base64, using the URL-friendly character set: case-sensitive letters, digits and the characters <code class="docutils literal notranslate"><span class="pre">_</span></code> and <code class="docutils literal notranslate"><span class="pre">-</span></code>.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.byte_length">
<em class="property">property </em><code class="sig-name descname">byte_length</code><a class="headerlink" href="#pulumi_random.RandomId.byte_length" title="Permalink to this definition">¶</a></dt>
<dd><p>The number of random bytes to produce. The
minimum value is 1, which produces eight bits of randomness.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.dec">
<em class="property">property </em><code class="sig-name descname">dec</code><a class="headerlink" href="#pulumi_random.RandomId.dec" title="Permalink to this definition">¶</a></dt>
<dd><p>The generated id presented in non-padded decimal digits.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.hex">
<em class="property">property </em><code class="sig-name descname">hex</code><a class="headerlink" href="#pulumi_random.RandomId.hex" title="Permalink to this definition">¶</a></dt>
<dd><p>The generated id presented in padded hexadecimal digits. This result will always be twice as long as the requested byte length.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.keepers">
<em class="property">property </em><code class="sig-name descname">keepers</code><a class="headerlink" href="#pulumi_random.RandomId.keepers" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.prefix">
<em class="property">property </em><code class="sig-name descname">prefix</code><a class="headerlink" href="#pulumi_random.RandomId.prefix" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary string to prefix the output value with. This
string is supplied as-is, meaning it is not guaranteed to be URL-safe or
base64 encoded.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomId.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomId.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomId.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomInteger">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomInteger</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">max</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">seed</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomInteger" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource <code class="docutils literal notranslate"><span class="pre">RandomInteger</span></code> generates random values from a given range, described by the <code class="docutils literal notranslate"><span class="pre">min</span></code> and <code class="docutils literal notranslate"><span class="pre">max</span></code> attributes of a given resource.</p>
<p>This resource can be used in conjunction with resources that have
the <code class="docutils literal notranslate"><span class="pre">create_before_destroy</span></code> lifecycle flag set, to avoid conflicts with
unique names during the brief period where both the old and new resources
exist concurrently.</p>
<p>The following example shows how to generate a random priority between 1 and 50000 for
a <code class="docutils literal notranslate"><span class="pre">aws_alb_listener_rule</span></code> resource:</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_aws</span> <span class="k">as</span> <span class="nn">aws</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">priority</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomInteger</span><span class="p">(</span><span class="s2">&quot;priority&quot;</span><span class="p">,</span>
    <span class="n">keepers</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;listener_arn&quot;</span><span class="p">:</span> <span class="n">var</span><span class="p">[</span><span class="s2">&quot;listener_arn&quot;</span><span class="p">],</span>
    <span class="p">},</span>
    <span class="nb">max</span><span class="o">=</span><span class="mi">50000</span><span class="p">,</span>
    <span class="nb">min</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
<span class="n">main</span> <span class="o">=</span> <span class="n">aws</span><span class="o">.</span><span class="n">alb</span><span class="o">.</span><span class="n">ListenerRule</span><span class="p">(</span><span class="s2">&quot;main&quot;</span><span class="p">,</span>
    <span class="n">actions</span><span class="o">=</span><span class="p">[</span><span class="n">aws</span><span class="o">.</span><span class="n">alb</span><span class="o">.</span><span class="n">ListenerRuleActionArgs</span><span class="p">(</span>
        <span class="n">target_group_arn</span><span class="o">=</span><span class="n">var</span><span class="p">[</span><span class="s2">&quot;target_group_arn&quot;</span><span class="p">],</span>
        <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;forward&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">listener_arn</span><span class="o">=</span><span class="n">var</span><span class="p">[</span><span class="s2">&quot;listener_arn&quot;</span><span class="p">],</span>
    <span class="n">priority</span><span class="o">=</span><span class="n">priority</span><span class="o">.</span><span class="n">result</span><span class="p">)</span>
</pre></div>
</div>
<p>The result of the above will set a random priority.</p>
<p>Random integers can be imported using the <code class="docutils literal notranslate"><span class="pre">result</span></code>, <code class="docutils literal notranslate"><span class="pre">min</span></code>, and <code class="docutils literal notranslate"><span class="pre">max</span></code>, with an optional <code class="docutils literal notranslate"><span class="pre">seed</span></code>. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example (values are separated by a <code class="docutils literal notranslate"><span class="pre">,</span></code>)</p>
<div class="highlight-sh notranslate"><div class="highlight"><pre><span></span>$ pulumi import random:index/randomInteger:RandomInteger priority <span class="m">15390</span>,1,50000
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>max</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The maximum inclusive value of the range.</p></li>
<li><p><strong>min</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The minimum inclusive value of the range.</p></li>
<li><p><strong>seed</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A custom seed to always produce the same value.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomInteger.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">max</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">result</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">seed</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_integer.RandomInteger<a class="headerlink" href="#pulumi_random.RandomInteger.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomInteger resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>max</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The maximum inclusive value of the range.</p></li>
<li><p><strong>min</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The minimum inclusive value of the range.</p></li>
<li><p><strong>result</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (int) The random Integer result.</p></li>
<li><p><strong>seed</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A custom seed to always produce the same value.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.keepers">
<em class="property">property </em><code class="sig-name descname">keepers</code><a class="headerlink" href="#pulumi_random.RandomInteger.keepers" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.max">
<em class="property">property </em><code class="sig-name descname">max</code><a class="headerlink" href="#pulumi_random.RandomInteger.max" title="Permalink to this definition">¶</a></dt>
<dd><p>The maximum inclusive value of the range.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.min">
<em class="property">property </em><code class="sig-name descname">min</code><a class="headerlink" href="#pulumi_random.RandomInteger.min" title="Permalink to this definition">¶</a></dt>
<dd><p>The minimum inclusive value of the range.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.result">
<em class="property">property </em><code class="sig-name descname">result</code><a class="headerlink" href="#pulumi_random.RandomInteger.result" title="Permalink to this definition">¶</a></dt>
<dd><p>(int) The random Integer result.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.seed">
<em class="property">property </em><code class="sig-name descname">seed</code><a class="headerlink" href="#pulumi_random.RandomInteger.seed" title="Permalink to this definition">¶</a></dt>
<dd><p>A custom seed to always produce the same value.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomInteger.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomInteger.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomInteger.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomPassword">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomPassword</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">lower</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_lower</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_numeric</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_special</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_upper</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">number</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">override_special</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">special</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">upper</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomPassword" title="Permalink to this definition">¶</a></dt>
<dd><p>Identical to the <code class="docutils literal notranslate"><span class="pre">RandomString</span></code> resource with the exception that the
result is treated as sensitive and, thus, <em>not</em> displayed in console output.</p>
<blockquote>
<div><p><strong>Note:</strong> All attributes including the generated password will be stored in
the raw state as plain-text.</p>
</div></blockquote>
<p>This resource <em>does</em> use a cryptographic random number generator.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_aws</span> <span class="k">as</span> <span class="nn">aws</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">password</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomPassword</span><span class="p">(</span><span class="s2">&quot;password&quot;</span><span class="p">,</span>
    <span class="n">length</span><span class="o">=</span><span class="mi">16</span><span class="p">,</span>
    <span class="n">special</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
    <span class="n">override_special</span><span class="o">=</span><span class="s2">&quot;_%@&quot;</span><span class="p">)</span>
<span class="n">example</span> <span class="o">=</span> <span class="n">aws</span><span class="o">.</span><span class="n">rds</span><span class="o">.</span><span class="n">Instance</span><span class="p">(</span><span class="s2">&quot;example&quot;</span><span class="p">,</span>
    <span class="n">instance_class</span><span class="o">=</span><span class="s2">&quot;db.t3.micro&quot;</span><span class="p">,</span>
    <span class="n">allocated_storage</span><span class="o">=</span><span class="mi">64</span><span class="p">,</span>
    <span class="n">engine</span><span class="o">=</span><span class="s2">&quot;mysql&quot;</span><span class="p">,</span>
    <span class="n">username</span><span class="o">=</span><span class="s2">&quot;someone&quot;</span><span class="p">,</span>
    <span class="n">password</span><span class="o">=</span><span class="n">password</span><span class="o">.</span><span class="n">result</span><span class="p">)</span>
</pre></div>
</div>
<p>Random Password can be imported by specifying the value of the string</p>
<div class="highlight-sh notranslate"><div class="highlight"><pre><span></span>$ pulumi import random:index/randomPassword:RandomPassword password securepassword
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomPassword.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">lower</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_lower</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_numeric</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_special</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_upper</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">number</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">override_special</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">result</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">special</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">upper</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_password.RandomPassword<a class="headerlink" href="#pulumi_random.RandomPassword.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomPassword resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPassword.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomPassword.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPassword.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomPassword.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomPet">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomPet</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">prefix</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">separator</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomPet" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource <code class="docutils literal notranslate"><span class="pre">RandomPet</span></code> generates random pet names that are intended to be
used as unique identifiers for other resources.</p>
<p>This resource can be used in conjunction with resources that have
the <code class="docutils literal notranslate"><span class="pre">create_before_destroy</span></code> lifecycle flag set, to avoid conflicts with
unique names during the brief period where both the old and new resources
exist concurrently.</p>
<p>The following example shows how to generate a unique pet name for an AWS EC2
instance that changes each time a new AMI id is selected.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_aws</span> <span class="k">as</span> <span class="nn">aws</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">server_random_pet</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomPet</span><span class="p">(</span><span class="s2">&quot;serverRandomPet&quot;</span><span class="p">,</span> <span class="n">keepers</span><span class="o">=</span><span class="p">{</span>
    <span class="s2">&quot;ami_id&quot;</span><span class="p">:</span> <span class="n">var</span><span class="p">[</span><span class="s2">&quot;ami_id&quot;</span><span class="p">],</span>
<span class="p">})</span>
<span class="n">server_instance</span> <span class="o">=</span> <span class="n">aws</span><span class="o">.</span><span class="n">ec2</span><span class="o">.</span><span class="n">Instance</span><span class="p">(</span><span class="s2">&quot;serverInstance&quot;</span><span class="p">,</span>
    <span class="n">ami</span><span class="o">=</span><span class="n">server_random_pet</span><span class="o">.</span><span class="n">keepers</span><span class="p">[</span><span class="s2">&quot;amiId&quot;</span><span class="p">],</span>
    <span class="n">tags</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;Name&quot;</span><span class="p">:</span> <span class="n">server_random_pet</span><span class="o">.</span><span class="n">id</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="nb">id</span><span class="p">:</span> <span class="sa">f</span><span class="s2">&quot;web-server-</span><span class="si">{</span><span class="nb">id</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">),</span>
    <span class="p">})</span>
</pre></div>
</div>
<p>The result of the above will set the Name of the AWS Instance to
<code class="docutils literal notranslate"><span class="pre">web-server-simple-snake</span></code>.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>length</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The length (in words) of the pet name.</p></li>
<li><p><strong>prefix</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A string to prefix the name with.</p></li>
<li><p><strong>separator</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The character to separate words in the pet name.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomPet.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">prefix</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">separator</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_pet.RandomPet<a class="headerlink" href="#pulumi_random.RandomPet.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomPet resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>length</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The length (in words) of the pet name.</p></li>
<li><p><strong>prefix</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A string to prefix the name with.</p></li>
<li><p><strong>separator</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The character to separate words in the pet name.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPet.keepers">
<em class="property">property </em><code class="sig-name descname">keepers</code><a class="headerlink" href="#pulumi_random.RandomPet.keepers" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPet.length">
<em class="property">property </em><code class="sig-name descname">length</code><a class="headerlink" href="#pulumi_random.RandomPet.length" title="Permalink to this definition">¶</a></dt>
<dd><p>The length (in words) of the pet name.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPet.prefix">
<em class="property">property </em><code class="sig-name descname">prefix</code><a class="headerlink" href="#pulumi_random.RandomPet.prefix" title="Permalink to this definition">¶</a></dt>
<dd><p>A string to prefix the name with.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPet.separator">
<em class="property">property </em><code class="sig-name descname">separator</code><a class="headerlink" href="#pulumi_random.RandomPet.separator" title="Permalink to this definition">¶</a></dt>
<dd><p>The character to separate words in the pet name.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPet.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomPet.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomPet.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomPet.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomShuffle">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomShuffle</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">inputs</span><span class="p">:</span> <span class="n">Union[Sequence[Union[str, Awaitable[str], Output[T]]], Awaitable[Sequence[Union[str, Awaitable[str], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">result_count</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">seed</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomShuffle" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource <code class="docutils literal notranslate"><span class="pre">RandomShuffle</span></code> generates a random permutation of a list
of strings given as an argument.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_aws</span> <span class="k">as</span> <span class="nn">aws</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">az</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomShuffle</span><span class="p">(</span><span class="s2">&quot;az&quot;</span><span class="p">,</span>
    <span class="n">inputs</span><span class="o">=</span><span class="p">[</span>
        <span class="s2">&quot;us-west-1a&quot;</span><span class="p">,</span>
        <span class="s2">&quot;us-west-1c&quot;</span><span class="p">,</span>
        <span class="s2">&quot;us-west-1d&quot;</span><span class="p">,</span>
        <span class="s2">&quot;us-west-1e&quot;</span><span class="p">,</span>
    <span class="p">],</span>
    <span class="n">result_count</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
<span class="n">example</span> <span class="o">=</span> <span class="n">aws</span><span class="o">.</span><span class="n">elb</span><span class="o">.</span><span class="n">LoadBalancer</span><span class="p">(</span><span class="s2">&quot;example&quot;</span><span class="p">,</span> <span class="n">availability_zones</span><span class="o">=</span><span class="n">az</span><span class="o">.</span><span class="n">results</span><span class="p">)</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>inputs</strong> (<em>pulumi.Input</em><em>[</em><em>Sequence</em><em>[</em><em>pulumi.Input</em><em>[</em><em>str</em><em>]</em><em>]</em><em>]</em>) – The list of strings to shuffle.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>result_count</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The number of results to return. Defaults to
the number of items in the <code class="docutils literal notranslate"><span class="pre">input</span></code> list. If fewer items are requested,
some elements will be excluded from the result. If more items are requested,
items will be repeated in the result but not more frequently than the number
of items in the input list.</p></li>
<li><p><strong>seed</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Arbitrary string with which to seed the random number
generator, in order to produce less-volatile permutations of the list.
<strong>Important:</strong> Even with an identical seed, it is not guaranteed that the
same permutation will be produced across different versions of the provider.
This argument causes the result to be <em>less volatile</em>, but not fixed for
all time.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomShuffle.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">inputs</span><span class="p">:</span> <span class="n">Union[Sequence[Union[str, Awaitable[str], Output[T]]], Awaitable[Sequence[Union[str, Awaitable[str], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">result_count</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">results</span><span class="p">:</span> <span class="n">Union[Sequence[Union[str, Awaitable[str], Output[T]]], Awaitable[Sequence[Union[str, Awaitable[str], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">seed</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_shuffle.RandomShuffle<a class="headerlink" href="#pulumi_random.RandomShuffle.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomShuffle resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>inputs</strong> (<em>pulumi.Input</em><em>[</em><em>Sequence</em><em>[</em><em>pulumi.Input</em><em>[</em><em>str</em><em>]</em><em>]</em><em>]</em>) – The list of strings to shuffle.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>result_count</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The number of results to return. Defaults to
the number of items in the <code class="docutils literal notranslate"><span class="pre">input</span></code> list. If fewer items are requested,
some elements will be excluded from the result. If more items are requested,
items will be repeated in the result but not more frequently than the number
of items in the input list.</p></li>
<li><p><strong>results</strong> (<em>pulumi.Input</em><em>[</em><em>Sequence</em><em>[</em><em>pulumi.Input</em><em>[</em><em>str</em><em>]</em><em>]</em><em>]</em>) – Random permutation of the list of strings given in <code class="docutils literal notranslate"><span class="pre">input</span></code>.</p></li>
<li><p><strong>seed</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Arbitrary string with which to seed the random number
generator, in order to produce less-volatile permutations of the list.
<strong>Important:</strong> Even with an identical seed, it is not guaranteed that the
same permutation will be produced across different versions of the provider.
This argument causes the result to be <em>less volatile</em>, but not fixed for
all time.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.inputs">
<em class="property">property </em><code class="sig-name descname">inputs</code><a class="headerlink" href="#pulumi_random.RandomShuffle.inputs" title="Permalink to this definition">¶</a></dt>
<dd><p>The list of strings to shuffle.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.keepers">
<em class="property">property </em><code class="sig-name descname">keepers</code><a class="headerlink" href="#pulumi_random.RandomShuffle.keepers" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.result_count">
<em class="property">property </em><code class="sig-name descname">result_count</code><a class="headerlink" href="#pulumi_random.RandomShuffle.result_count" title="Permalink to this definition">¶</a></dt>
<dd><p>The number of results to return. Defaults to
the number of items in the <code class="docutils literal notranslate"><span class="pre">input</span></code> list. If fewer items are requested,
some elements will be excluded from the result. If more items are requested,
items will be repeated in the result but not more frequently than the number
of items in the input list.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.results">
<em class="property">property </em><code class="sig-name descname">results</code><a class="headerlink" href="#pulumi_random.RandomShuffle.results" title="Permalink to this definition">¶</a></dt>
<dd><p>Random permutation of the list of strings given in <code class="docutils literal notranslate"><span class="pre">input</span></code>.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.seed">
<em class="property">property </em><code class="sig-name descname">seed</code><a class="headerlink" href="#pulumi_random.RandomShuffle.seed" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary string with which to seed the random number
generator, in order to produce less-volatile permutations of the list.
<strong>Important:</strong> Even with an identical seed, it is not guaranteed that the
same permutation will be produced across different versions of the provider.
This argument causes the result to be <em>less volatile</em>, but not fixed for
all time.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomShuffle.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomShuffle.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomShuffle.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomString">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomString</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">lower</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_lower</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_numeric</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_special</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_upper</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">number</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">override_special</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">special</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">upper</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomString" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource <code class="docutils literal notranslate"><span class="pre">RandomString</span></code> generates a random permutation of alphanumeric
characters and optionally special characters.</p>
<p>This resource <em>does</em> use a cryptographic random number generator.</p>
<p>Historically this resource’s intended usage has been ambiguous as the original example
used it in a password. For backwards compatibility it will
continue to exist. For unique ids please use the <code class="docutils literal notranslate"><span class="pre">RandomId</span></code> resource, for sensitive
random values please use the <code class="docutils literal notranslate"><span class="pre">RandomPassword</span></code> resource.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">random</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomString</span><span class="p">(</span><span class="s2">&quot;random&quot;</span><span class="p">,</span>
    <span class="n">length</span><span class="o">=</span><span class="mi">16</span><span class="p">,</span>
    <span class="n">override_special</span><span class="o">=</span><span class="s2">&quot;/@£$&quot;</span><span class="p">,</span>
    <span class="n">special</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
</pre></div>
</div>
<p>Strings can be imported by just specifying the value of the string</p>
<div class="highlight-sh notranslate"><div class="highlight"><pre><span></span>$ pulumi import random:index/randomString:RandomString <span class="nb">test</span> <span class="nb">test</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>length</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The length of the string desired</p></li>
<li><p><strong>lower</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include lowercase alphabet characters
in random string.</p></li>
<li><p><strong>min_lower</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of lowercase alphabet
characters in random string.</p></li>
<li><p><strong>min_numeric</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of numeric characters
in random string.</p></li>
<li><p><strong>min_special</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of special characters
in random string.</p></li>
<li><p><strong>min_upper</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of uppercase alphabet
characters in random string.</p></li>
<li><p><strong>number</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include numeric characters in random
string.</p></li>
<li><p><strong>override*special</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Supply your own list of special characters to
use for string generation.  This overrides the default character list in the special
argument.  The special argument must still be set to true for any overwritten
characters to be used in generation.</p>
</p></li>
<li><p><strong>special</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include special characters in random
string. These are <cite>!&#64;#$%&amp;*()-*=+[]{}&lt;&gt;:?</cite></p></li>
<li><p><strong>upper</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include uppercase alphabet characters
in random string.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomString.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">length</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">lower</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_lower</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_numeric</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_special</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">min_upper</span><span class="p">:</span> <span class="n">Union[int, Awaitable[int], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">number</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">override_special</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">result</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">special</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">upper</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_string.RandomString<a class="headerlink" href="#pulumi_random.RandomString.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomString resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p></li>
<li><p><strong>length</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – The length of the string desired</p></li>
<li><p><strong>lower</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include lowercase alphabet characters
in random string.</p></li>
<li><p><strong>min_lower</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of lowercase alphabet
characters in random string.</p></li>
<li><p><strong>min_numeric</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of numeric characters
in random string.</p></li>
<li><p><strong>min_special</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of special characters
in random string.</p></li>
<li><p><strong>min_upper</strong> (<em>pulumi.Input</em><em>[</em><em>int</em><em>]</em>) – (default 0) Minimum number of uppercase alphabet
characters in random string.</p></li>
<li><p><strong>number</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include numeric characters in random
string.</p></li>
<li><p><strong>override*special</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Supply your own list of special characters to
use for string generation.  This overrides the default character list in the special
argument.  The special argument must still be set to true for any overwritten
characters to be used in generation.</p>
</p></li>
<li><p><strong>result</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Random string generated.</p></li>
<li><p><strong>special</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include special characters in random
string. These are <cite>!&#64;#$%&amp;*()-*=+[]{}&lt;&gt;:?</cite></p></li>
<li><p><strong>upper</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – (default true) Include uppercase alphabet characters
in random string.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.keepers">
<em class="property">property </em><code class="sig-name descname">keepers</code><a class="headerlink" href="#pulumi_random.RandomString.keepers" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary map of values that, when changed, will
trigger a new id to be generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.length">
<em class="property">property </em><code class="sig-name descname">length</code><a class="headerlink" href="#pulumi_random.RandomString.length" title="Permalink to this definition">¶</a></dt>
<dd><p>The length of the string desired</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.lower">
<em class="property">property </em><code class="sig-name descname">lower</code><a class="headerlink" href="#pulumi_random.RandomString.lower" title="Permalink to this definition">¶</a></dt>
<dd><p>(default true) Include lowercase alphabet characters
in random string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.min_lower">
<em class="property">property </em><code class="sig-name descname">min_lower</code><a class="headerlink" href="#pulumi_random.RandomString.min_lower" title="Permalink to this definition">¶</a></dt>
<dd><p>(default 0) Minimum number of lowercase alphabet
characters in random string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.min_numeric">
<em class="property">property </em><code class="sig-name descname">min_numeric</code><a class="headerlink" href="#pulumi_random.RandomString.min_numeric" title="Permalink to this definition">¶</a></dt>
<dd><p>(default 0) Minimum number of numeric characters
in random string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.min_special">
<em class="property">property </em><code class="sig-name descname">min_special</code><a class="headerlink" href="#pulumi_random.RandomString.min_special" title="Permalink to this definition">¶</a></dt>
<dd><p>(default 0) Minimum number of special characters
in random string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.min_upper">
<em class="property">property </em><code class="sig-name descname">min_upper</code><a class="headerlink" href="#pulumi_random.RandomString.min_upper" title="Permalink to this definition">¶</a></dt>
<dd><p>(default 0) Minimum number of uppercase alphabet
characters in random string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.number">
<em class="property">property </em><code class="sig-name descname">number</code><a class="headerlink" href="#pulumi_random.RandomString.number" title="Permalink to this definition">¶</a></dt>
<dd><p>(default true) Include numeric characters in random
string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.override_special">
<em class="property">property </em><code class="sig-name descname">override_special</code><a class="headerlink" href="#pulumi_random.RandomString.override_special" title="Permalink to this definition">¶</a></dt>
<dd><p>Supply your own list of special characters to
use for string generation.  This overrides the default character list in the special
argument.  The special argument must still be set to true for any overwritten
characters to be used in generation.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.result">
<em class="property">property </em><code class="sig-name descname">result</code><a class="headerlink" href="#pulumi_random.RandomString.result" title="Permalink to this definition">¶</a></dt>
<dd><p>Random string generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.special">
<em class="property">property </em><code class="sig-name descname">special</code><a class="headerlink" href="#pulumi_random.RandomString.special" title="Permalink to this definition">¶</a></dt>
<dd><p>(default true) Include special characters in random
string. These are <code class="docutils literal notranslate"><span class="pre">!&#64;#$%&amp;*()-_=+[]{}&lt;&gt;:?</span></code></p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.upper">
<em class="property">property </em><code class="sig-name descname">upper</code><a class="headerlink" href="#pulumi_random.RandomString.upper" title="Permalink to this definition">¶</a></dt>
<dd><p>(default true) Include uppercase alphabet characters
in random string.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomString.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomString.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomString.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_random.RandomUuid">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_random.</code><code class="sig-name descname">RandomUuid</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomUuid" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource <code class="docutils literal notranslate"><span class="pre">RandomUuid</span></code> generates random uuid string that is intended to be
used as unique identifiers for other resources.</p>
<p>This resource uses the <code class="docutils literal notranslate"><span class="pre">hashicorp/go-uuid</span></code> to generate a UUID-formatted string
for use with services needed a unique string identifier.</p>
<p>The following example shows how to generate a unique name for an Azure Resource Group.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_azure</span> <span class="k">as</span> <span class="nn">azure</span>
<span class="kn">import</span> <span class="nn">pulumi_random</span> <span class="k">as</span> <span class="nn">random</span>

<span class="n">test_random_uuid</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">RandomUuid</span><span class="p">(</span><span class="s2">&quot;testRandomUuid&quot;</span><span class="p">)</span>
<span class="n">test_resource_group</span> <span class="o">=</span> <span class="n">azure</span><span class="o">.</span><span class="n">core</span><span class="o">.</span><span class="n">ResourceGroup</span><span class="p">(</span><span class="s2">&quot;testResourceGroup&quot;</span><span class="p">,</span> <span class="n">location</span><span class="o">=</span><span class="s2">&quot;Central US&quot;</span><span class="p">)</span>
</pre></div>
</div>
<p>Random UUID’s can be imported. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example</p>
<div class="highlight-sh notranslate"><div class="highlight"><pre><span></span>$ pulumi import random:index/randomUuid:RandomUuid main aabbccdd-eeff-0011-2233-445566778899
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new uuid to be generated.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_random.RandomUuid.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">keepers</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">result</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_random.random_uuid.RandomUuid<a class="headerlink" href="#pulumi_random.RandomUuid.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing RandomUuid resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>keepers</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – Arbitrary map of values that, when changed, will
trigger a new uuid to be generated.</p></li>
<li><p><strong>result</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The generated uuid presented in string format.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomUuid.keepers">
<em class="property">property </em><code class="sig-name descname">keepers</code><a class="headerlink" href="#pulumi_random.RandomUuid.keepers" title="Permalink to this definition">¶</a></dt>
<dd><p>Arbitrary map of values that, when changed, will
trigger a new uuid to be generated.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomUuid.result">
<em class="property">property </em><code class="sig-name descname">result</code><a class="headerlink" href="#pulumi_random.RandomUuid.result" title="Permalink to this definition">¶</a></dt>
<dd><p>The generated uuid presented in string format.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomUuid.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomUuid.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_random.RandomUuid.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_random.RandomUuid.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

</div>
