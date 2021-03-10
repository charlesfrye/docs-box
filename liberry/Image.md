description: Wandb class for images.
robots: noindex

# liberry.Image

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>



Wandb class for images.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>liberry.Image(
    data_or_path: "ImageDataOrPathType",
    mode: Optional[str] = None,
    caption: Optional[str] = None,
    grouping: Optional[str] = None,
    classes: Optional[Union['Classes', Sequence[dict]]] = None,
    boxes: Optional[Union[Dict[str, 'BoundingBoxes2D'], Dict[str, dict]]] = None,
    masks: Optional[Union[Dict[str, 'ImageMask'], Dict[str, dict]]] = None
) -> None
</code></pre>



<!-- Placeholder for "Used in" -->


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Arguments</h2></th></tr>

<tr>
<td>
`data_or_path`
</td>
<td>
(numpy array, string, io) Accepts numpy array of
image data, or a PIL image. The class attempts to infer
the data format and converts it.
</td>
</tr><tr>
<td>
`mode`
</td>
<td>
(string) The PIL mode for an image. Most common are "L", "RGB",
"RGBA". Full explanation at https://pillow.readthedocs.io/en/4.2.x/handbook/concepts.html#concept-modes.
</td>
</tr><tr>
<td>
`caption`
</td>
<td>
(string) Label for display of image.
</td>
</tr>
</table>



## Methods

<h3 id="all_boxes"><code>all_boxes</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>@classmethod</code>
<code>all_boxes(
    images: Sequence['Image'],
    run: "LocalRun",
    run_key: str,
    step: Union[int, str]
) -> Union[List[Optional[dict]], bool]
</code></pre>




<h3 id="all_captions"><code>all_captions</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>@classmethod</code>
<code>all_captions(
    images: Sequence['Media']
) -> Union[bool, Sequence[Optional[str]]]
</code></pre>




<h3 id="all_masks"><code>all_masks</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>@classmethod</code>
<code>all_masks(
    images: Sequence['Image'],
    run: "LocalRun",
    run_key: str,
    step: Union[int, str]
) -> Union[List[Optional[dict]], bool]
</code></pre>




<h3 id="guess_mode"><code>guess_mode</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>guess_mode(
    data: "np.ndarray"
) -> str
</code></pre>

Guess what type of image the np.array is representing


<h3 id="to_uint8"><code>to_uint8</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>@classmethod</code>
<code>to_uint8(
    data: "np.ndarray"
) -> "np.ndarray"
</code></pre>

Converts floating point image on the range [0,1] and integer images
on the range [0,255] to uint8, clipping if necessary.





<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Class Variables</h2></th></tr>

<tr>
<td>
MAX_DIMENSION<a id="MAX_DIMENSION"></a>
</td>
<td>
`65500`
</td>
</tr><tr>
<td>
MAX_ITEMS<a id="MAX_ITEMS"></a>
</td>
<td>
`108`
</td>
</tr><tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`'image-file'`
</td>
</tr>
</table>

