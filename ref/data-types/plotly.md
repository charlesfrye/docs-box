# Plotly



[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/3a0def97afe1def2b1a59786b4f0bbcac3f5dc4c/wandb/sdk/data_types.py#L1923-L1970)




Wandb class for plotly plots.

<pre><code>Plotly(
    val: Union['plotly.Figure', 'matplotlib.artist.Artist']
)</code></pre>





<!-- Tabular view -->
<table>
<tr><th>Arguments</th></tr>

<tr>
<td>
<code>val</code>
</td>
<td>
matplotlib or plotly figure
</td>
</tr>
</table>



## Methods

<h3 id="make_plot_media"><code>make_plot_media</code></h3>

<a target="_blank" href="https://www.github.com/wandb/client/tree/3a0def97afe1def2b1a59786b4f0bbcac3f5dc4c/wandb/sdk/data_types.py#L1931-L1939">View source</a>

<pre><code>@classmethod</code>
<code>make_plot_media(
    val: Union['plotly.Figure', 'matplotlib.artist.Artist']
) -> Union[Image, 'Plotly']</code></pre>








<!-- Tabular view -->
<table>
<tr><th>Class Variables</th></tr>

<tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
<code>None</code>
</td>
</tr>
</table>

