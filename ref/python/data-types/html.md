# Html



[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/sdk/data_types.py#L869-L959)




Wandb class for arbitrary html

<pre><code>Html(
    data: Union[str, 'TextIO'],
    inject: bool = (True)
) -> None</code></pre>





<!-- Tabular view -->
<table>
<tr><th>Arguments</th></tr>

<tr>
<td>
<code>data</code>
</td>
<td>
(string or io object) HTML to display in wandb
</td>
</tr><tr>
<td>
<code>inject</code>
</td>
<td>
(boolean) Add a stylesheet to the HTML object.  If set
to False the HTML will pass through unchanged.
</td>
</tr>
</table>



## Methods

<h3 id="inject_head"><code>inject_head</code></h3>

<a target="_blank" href="https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/sdk/data_types.py#L911-L926">View source</a>

<pre><code>inject_head() -> None</code></pre>








<!-- Tabular view -->
<table>
<tr><th>Class Variables</th></tr>

<tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`'html-file'`
</td>
</tr>
</table>

