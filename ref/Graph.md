# Graph

<!-- Insert buttons and diff -->


[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/master/wandb/data_types.py#L851-L1009)




Wandb class for graphs

<pre><code>Graph(
    format=&#x27;keras&#x27;
)</code></pre>



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

<a target="_blank" href="https://www.github.com/wandb/client/tree/master/wandb/data_types.py#L935-L939">View source</a>

<pre><code>add_edge(
    from_node, to_node
)</code></pre>




<h3 id="add_node"><code>add_node</code></h3>

<a target="_blank" href="https://www.github.com/wandb/client/tree/master/wandb/data_types.py#L921-L933">View source</a>

<pre><code>add_node(
    node=None, **node_kwargs
)</code></pre>




<h3 id="from_keras"><code>from_keras</code></h3>

<a target="_blank" href="https://www.github.com/wandb/client/tree/master/wandb/data_types.py#L941-L970">View source</a>

<pre><code>@classmethod</code>
<code>from_keras(
    model
)</code></pre>




<h3 id="pprint"><code>pprint</code></h3>

<a target="_blank" href="https://www.github.com/wandb/client/tree/master/wandb/data_types.py#L915-L919">View source</a>

<pre><code>pprint()</code></pre>




<h3 id="__getitem__"><code>__getitem__</code></h3>

<a target="_blank" href="https://www.github.com/wandb/client/tree/master/wandb/data_types.py#L912-L913">View source</a>

<pre><code>__getitem__(
    nid
)</code></pre>








<!-- Tabular view -->
<table>
<tr><th>Class Variables</th></tr>

<tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`None`
</td>
</tr>
</table>

