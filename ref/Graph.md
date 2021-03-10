description: Wandb class for graphs
robots: noindex

# ref.Graph

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>



Wandb class for graphs

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>ref.Graph(
    format=&#x27;keras&#x27;
)
</code></pre>



<!-- Placeholder for "Used in" -->

This class is typically used for saving and diplaying neural net models.  It
represents the graph as an array of nodes and edges.  The nodes can have
labels that can be visualized by wandb.

#### Examples:

Import a keras model:
```
    Graph.from_keras(keras_model)
```



## Methods

<h3 id="add_edge"><code>add_edge</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>add_edge(
    from_node, to_node
)
</code></pre>




<h3 id="add_node"><code>add_node</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>add_node(
    node=None, **node_kwargs
)
</code></pre>




<h3 id="from_keras"><code>from_keras</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>@classmethod</code>
<code>from_keras(
    model
)
</code></pre>




<h3 id="pprint"><code>pprint</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>pprint()
</code></pre>




<h3 id="__getitem__"><code>__getitem__</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>__getitem__(
    nid
)
</code></pre>








<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Class Variables</h2></th></tr>

<tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`None`
</td>
</tr>
</table>

