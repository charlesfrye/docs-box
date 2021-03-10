description: Wandb class for arbitrary html
robots: noindex

# ref.Html

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>



Wandb class for arbitrary html

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>ref.Html(
    data: Union[str, 'TextIO'],
    inject: bool = True
) -> None
</code></pre>



<!-- Placeholder for "Used in" -->


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Arguments</h2></th></tr>

<tr>
<td>
`data`
</td>
<td>
(string or io object) HTML to display in wandb
</td>
</tr><tr>
<td>
`inject`
</td>
<td>
(boolean) Add a stylesheet to the HTML object.  If set
to False the HTML will pass through unchanged.
</td>
</tr>
</table>



## Methods

<h3 id="inject_head"><code>inject_head</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>inject_head() -> None
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
`'html-file'`
</td>
</tr>
</table>

