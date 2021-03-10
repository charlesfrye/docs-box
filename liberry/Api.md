description: Used for querying the wandb server.
robots: noindex

# liberry.Api

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>



Used for querying the wandb server.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>liberry.Api(
    overrides={}
)
</code></pre>



<!-- Placeholder for "Used in" -->


#### Examples:

Most common way to initialize
```
>>> wandb.Api()
```



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Arguments</h2></th></tr>

<tr>
<td>
`overrides`
</td>
<td>
(dict) You can set `base_url` if you are using a wandb server
other than https://api.wandb.ai.
You can also set defaults for `entity`, `project`, and `run`.
</td>
</tr>
</table>





<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Attributes</h2></th></tr>

<tr>
<td>
`api_key`
</td>
<td>

</td>
</tr><tr>
<td>
`client`
</td>
<td>

</td>
</tr><tr>
<td>
`default_entity`
</td>
<td>

</td>
</tr><tr>
<td>
`user_agent`
</td>
<td>

</td>
</tr>
</table>



## Methods

<h3 id="artifact"><code>artifact</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>artifact(
    name, type=None
)
</code></pre>

Returns a single artifact by parsing path in the form `entity/project/run_id`.


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Arguments</th></tr>

<tr>
<td>
`name`
</td>
<td>
(str) An artifact name. May be prefixed with entity/project. Valid names
can be in the following forms:
name:version
name:alias
digest
</td>
</tr><tr>
<td>
`type`
</td>
<td>
(str, optional) The type of artifact to fetch.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="2">
A `Artifact` object.
</td>
</tr>

</table>



<h3 id="artifact_type"><code>artifact_type</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>artifact_type(
    type_name, project=None
)
</code></pre>




<h3 id="artifact_types"><code>artifact_types</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>artifact_types(
    project=None
)
</code></pre>




<h3 id="artifact_versions"><code>artifact_versions</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>artifact_versions(
    type_name, name, per_page=50
)
</code></pre>




<h3 id="create_run"><code>create_run</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>create_run(
    **kwargs
)
</code></pre>

Create a new run


<h3 id="flush"><code>flush</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>flush()
</code></pre>

The api object keeps a local cache of runs, so if the state of the run may
change while executing your script you must clear the local cache with `api.flush()`
to get the latest values associated with the run.

<h3 id="projects"><code>projects</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>projects(
    entity=None, per_page=200
)
</code></pre>

Get projects for a given entity.


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Arguments</th></tr>

<tr>
<td>
`entity`
</td>
<td>
(str) Name of the entity requested.  If None will fallback to
default entity passed to `Api`.  If no default entity, will raise a `ValueError`.
</td>
</tr><tr>
<td>
`per_page`
</td>
<td>
(int) Sets the page size for query pagination.  None will use the default size.
Usually there is no reason to change this.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="2">
A `Projects` object which is an iterable collection of `Project` objects.
</td>
</tr>

</table>



<h3 id="reports"><code>reports</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>reports(
    path=&#x27;&#x27;, name=None, per_page=50
)
</code></pre>

Get reports for a given project path.

WARNING: This api is in beta and will likely change in a future release

<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Arguments</th></tr>

<tr>
<td>
`path`
</td>
<td>
(str) path to project the report resides in, should be in the form: "entity/project"
</td>
</tr><tr>
<td>
`name`
</td>
<td>
(str) optional name of the report requested.
</td>
</tr><tr>
<td>
`per_page`
</td>
<td>
(int) Sets the page size for query pagination.  None will use the default size.
Usually there is no reason to change this.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="2">
A `Reports` object which is an iterable collection of `BetaReport` objects.
</td>
</tr>

</table>



<h3 id="run"><code>run</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>run(
    path=&#x27;&#x27;
)
</code></pre>

Returns a single run by parsing path in the form entity/project/run_id.


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Arguments</th></tr>

<tr>
<td>
`path`
</td>
<td>
(str) path to run in the form `entity/project/run_id`.
If api.entity is set, this can be in the form `project/run_id`
and if `api.project` is set this can just be the run_id.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="2">
A `Run` object.
</td>
</tr>

</table>



<h3 id="runs"><code>runs</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>runs(
    path=&#x27;&#x27;, filters=None, order=&#x27;-created_at&#x27;, per_page=50
)
</code></pre>

Return a set of runs from a project that match the filters provided.

You can filter by `config.*`, `summary.*`, `state`, `entity`, `createdAt`, etc.

#### Examples:

Find runs in my_project where config.experiment_name has been set to "foo"
```
api.runs(path="my_entity/my_project", filters={"config.experiment_name": "foo"})
```

Find runs in my_project where config.experiment_name has been set to "foo" or "bar"
```
api.runs(path="my_entity/my_project",
    filters={"$or": [{"config.experiment_name": "foo"}, {"config.experiment_name": "bar"}]})
```

Find runs in my_project where config.experiment_name matches a regex (anchors are not supported)
```
api.runs(path="my_entity/my_project",
    filters={"config.experiment_name": {"$regex": "b.*"}})
```

Find runs in my_project sorted by ascending loss
```
api.runs(path="my_entity/my_project", order="+summary_metrics.loss")
```



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Arguments</th></tr>

<tr>
<td>
`path`
</td>
<td>
(str) path to project, should be in the form: "entity/project"
</td>
</tr><tr>
<td>
`filters`
</td>
<td>
(dict) queries for specific runs using the MongoDB query language.
You can filter by run properties such as config.key, summary_metrics.key, state, entity, createdAt, etc.
For example: {"config.experiment_name": "foo"} would find runs with a config entry
of experiment name set to "foo"
You can compose operations to make more complicated queries,
see Reference for the language is at  https://docs.mongodb.com/manual/reference/operator/query
</td>
</tr><tr>
<td>
`order`
</td>
<td>
(str) Order can be `created_at`, `heartbeat_at`, `config.*.value`, or `summary_metrics.*`.
If you prepend order with a + order is ascending.
If you prepend order with a - order is descending (default).
The default order is run.created_at from newest to oldest.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="2">
A `Runs` object, which is an iterable collection of `Run` objects.
</td>
</tr>

</table>



<h3 id="sweep"><code>sweep</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>sweep(
    path=&#x27;&#x27;
)
</code></pre>

Returns a sweep by parsing path in the form `entity/project/sweep_id`.


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Arguments</th></tr>

<tr>
<td>
`path`
</td>
<td>
(str, optional) path to sweep in the form entity/project/sweep_id.  If api.entity
is set, this can be in the form project/sweep_id and if `api.project` is set
this can just be the sweep_id.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="2">
A `Sweep` object.
</td>
</tr>

</table>



<h3 id="sync_tensorboard"><code>sync_tensorboard</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/apis/public.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>sync_tensorboard(
    root_dir, run_id=None, project=None, entity=None
)
</code></pre>

Sync a local directory containing tfevent files to wandb






<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Class Variables</h2></th></tr>

<tr>
<td>
VIEWER_QUERY<a id="VIEWER_QUERY"></a>
</td>
<td>

</td>
</tr>
</table>

