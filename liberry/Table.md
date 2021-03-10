description: This is a table designed to display sets of records.
robots: noindex

# liberry.Table

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>



This is a table designed to display sets of records.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>liberry.Table(
    columns=None, data=None, rows=None, dataframe=None, dtype=None, optional=True,
    allow_mixed_types=False
)
</code></pre>



<!-- Placeholder for "Used in" -->


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Arguments</h2></th></tr>

<tr>
<td>
`columns`
</td>
<td>
([str]) Names of the columns in the table.
Defaults to ["Input", "Output", "Expected"].
</td>
</tr><tr>
<td>
`data`
</td>
<td>
(array) 2D Array of values that will be displayed as strings.
</td>
</tr><tr>
<td>
`dataframe`
</td>
<td>
(pandas.DataFrame) DataFrame object used to create the table.
When set, the other arguments are ignored.
optional (Union[bool,List[bool]]): If None values are allowed. Singular bool
applies to all columns. A list of bool values applies to each respective column.
Default to True.
allow_mixed_types (bool): Determines if columns are allowed to have mixed types (disables type validation). Defaults to False
</td>
</tr>
</table>



## Methods

<h3 id="add_data"><code>add_data</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>add_data(
    *data
)
</code></pre>

Add a row of data to the table. Argument length should match column length


<h3 id="add_row"><code>add_row</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>add_row(
    *row
)
</code></pre>




<h3 id="cast"><code>cast</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>cast(
    col_name, dtype, optional=False
)
</code></pre>




<h3 id="iterrows"><code>iterrows</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>iterrows()
</code></pre>

Iterate over rows as (ndx, row)
Yields
------
index : int
    The index of the row.
row : List[any]
    The data of the row





<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Class Variables</h2></th></tr>

<tr>
<td>
MAX_ARTIFACT_ROWS<a id="MAX_ARTIFACT_ROWS"></a>
</td>
<td>
`200000`
</td>
</tr><tr>
<td>
MAX_ROWS<a id="MAX_ROWS"></a>
</td>
<td>
`10000`
</td>
</tr><tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`'table'`
</td>
</tr>
</table>

