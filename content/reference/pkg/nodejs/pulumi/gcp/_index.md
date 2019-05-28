---
title: Package @pulumi/gcp
aliases:
    - "/reference/pkg/nodejs/@pulumi/gcp/"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


{{< langchoose nodeonly >}}

```javascript
var gcp = require("@pulumi/gcp");
```

```typescript
import * as gcp from "@pulumi/gcp";
```


<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Provider">class Provider</a></li>
<li><a href="#getEnv">function getEnv</a></li>
<li><a href="#getEnvBoolean">function getEnvBoolean</a></li>
<li><a href="#getEnvNumber">function getEnvNumber</a></li>
<li><a href="#ifUndefined">function ifUndefined</a></li>
<li><a href="#requireWithDefault">function requireWithDefault</a></li>
<li><a href="#ProviderArgs">interface ProviderArgs</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts">provider.ts</a> <a href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utilities.ts">utilities.ts</a> <a href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utils.ts">utils.ts</a> 
</div>
</div>
</div>

<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Modules">Modules ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Modules">Modules ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="accesscontextmanager">accesscontextmanager</a></li>
<li><a href="appengine">appengine</a></li>
<li><a href="bigquery">bigquery</a></li>
<li><a href="bigtable">bigtable</a></li>
<li><a href="billing">billing</a></li>
<li><a href="binaryauthorization">binaryauthorization</a></li>
<li><a href="cloudbuild">cloudbuild</a></li>
<li><a href="cloudfunctions">cloudfunctions</a></li>
<li><a href="cloudscheduler">cloudscheduler</a></li>
<li><a href="composer">composer</a></li>
<li><a href="compute">compute</a></li>
<li><a href="config">config</a></li>
<li><a href="container">container</a></li>
<li><a href="containeranalysis">containeranalysis</a></li>
<li><a href="dataflow">dataflow</a></li>
<li><a href="dataproc">dataproc</a></li>
<li><a href="dns">dns</a></li>
<li><a href="endpoints">endpoints</a></li>
<li><a href="filestore">filestore</a></li>
<li><a href="folder">folder</a></li>
<li><a href="iam">iam</a></li>
<li><a href="kms">kms</a></li>
<li><a href="logging">logging</a></li>
<li><a href="monitoring">monitoring</a></li>
<li><a href="organizations">organizations</a></li>
<li><a href="projects">projects</a></li>
<li><a href="pubsub">pubsub</a></li>
<li><a href="redis">redis</a></li>
<li><a href="resourcemanager">resourcemanager</a></li>
<li><a href="runtimeconfig">runtimeconfig</a></li>
<li><a href="serverless">serverless</a></li>
<li><a href="serviceAccount">serviceAccount</a></li>
<li><a href="servicenetworking">servicenetworking</a></li>
<li><a href="sourcerepo">sourcerepo</a></li>
<li><a href="spanner">spanner</a></li>
<li><a href="sql">sql</a></li>
<li><a href="storage">storage</a></li>
<li><a href="tpu">tpu</a></li>
</ul>
</div>
</div>
</div>

<h2 class="pdoc-module-header" id="Provider">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L13">class <b>Provider</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> ProviderResource</pre>

The provider type for the google-beta package. By default, resources use package-wide configuration
settings, however an explicit `Provider` instance may be created and passed during resource
construction to achieve fine-grained programmatic control over provider settings. See the
[documentation](https://pulumi.io/reference/programming-model.html#providers) for more information.

<h3 class="pdoc-member-header" id="Provider-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L13"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Provider(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: <a href='#ProviderArgs'>ProviderArgs</a>, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#ResourceOptions'>pulumi.ResourceOptions</a>)</pre>


Create a Provider resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Provider-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L14">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Provider-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L107">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Provider-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L102">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Provider-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L12">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="getEnv">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utilities.ts#L7">function <b>getEnv</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getEnv(vars: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[]): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="getEnvBoolean">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utilities.ts#L17">function <b>getEnvBoolean</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getEnvBoolean(vars: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[]): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="getEnvNumber">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utilities.ts#L32">function <b>getEnvNumber</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getEnvNumber(vars: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[]): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="ifUndefined">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utils.ts#L18">function <b>ifUndefined</b></a>
</h2>
<div class="pdoc-module-contents">
</div>
<h2 class="pdoc-module-header" id="requireWithDefault">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/utilities.ts#L43">function <b>requireWithDefault</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>requireWithDefault&lt;T&gt;(req: () => T, def: T | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>): T</pre>

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="ProviderArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L39">interface <b>ProviderArgs</b></a>
</h2>
<div class="pdoc-module-contents">

The set of arguments for constructing a Provider resource.

<h3 class="pdoc-member-header" id="ProviderArgs-accessToken">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L40">property <b>accessToken</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>accessToken?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="ProviderArgs-credentials">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L41">property <b>credentials</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>credentials?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="ProviderArgs-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L42">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="ProviderArgs-region">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L43">property <b>region</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>region?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="ProviderArgs-scopes">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L44">property <b>scopes</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>scopes?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="ProviderArgs-zone">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/dfd50d3cd37076dc64bfff16a687877050b08fcb/sdk/nodejs/provider.ts#L45">property <b>zone</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>zone?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>