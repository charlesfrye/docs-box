description: wandb class for histograms.
robots: noindex

# ref.Histogram

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>



wandb class for histograms.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>ref.Histogram(
    sequence: Optional[Sequence] = None,
    np_histogram: Optional['NumpyHistogram'] = None,
    num_bins: int = 64
) -> None
</code></pre>



<!-- Placeholder for "Used in" -->

This object works just like numpy's histogram function
https://docs.scipy.org/doc/numpy/reference/generated/numpy.histogram.html

#### Examples:

Generate histogram from a sequence
```python
wandb.Histogram([1,2,3])
```

Efficiently initialize from np.histogram.
```python
hist = np.histogram(data)
wandb.Histogram(np_histogram=hist)
```



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Arguments</h2></th></tr>

<tr>
<td>
`sequence`
</td>
<td>
(array_like) input data for histogram
</td>
</tr><tr>
<td>
`np_histogram`
</td>
<td>
(numpy histogram) alternative input of a precoomputed histogram
</td>
</tr><tr>
<td>
`num_bins`
</td>
<td>
(int) Number of bins for the histogram.  The default number of bins
is 64.  The maximum number of bins is 512
</td>
</tr>
</table>





<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Attributes</h2></th></tr>

<tr>
<td>
`bins`
</td>
<td>
([float]) edges of bins
</td>
</tr><tr>
<td>
`histogram`
</td>
<td>
([int]) number of elements falling in each bin
</td>
</tr>
</table>





<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Class Variables</h2></th></tr>

<tr>
<td>
MAX_LENGTH<a id="MAX_LENGTH"></a>
</td>
<td>
`512`
</td>
</tr><tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`None`
</td>
</tr>
</table>

