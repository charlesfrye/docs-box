description: Wandb representation of video.
robots: noindex

# liberry.Video

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>



Wandb representation of video.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>liberry.Video(
    data_or_path: Union['np.ndarray', str, 'TextIO'],
    caption: Optional[str] = None,
    fps: int = 4,
    format: Optional[str] = None
)
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
(numpy array, string, io)
Video can be initialized with a path to a file or an io object.
The format must be "gif", "mp4", "webm" or "ogg".
The format must be specified with the format argument.
Video can be initialized with a numpy tensor.
The numpy tensor must be either 4 dimensional or 5 dimensional.
Channels should be (time, channel, height, width) or
(batch, time, channel, height width)
</td>
</tr><tr>
<td>
`caption`
</td>
<td>
(string) caption associated with the video for display
</td>
</tr><tr>
<td>
`fps`
</td>
<td>
(int) frames per second for video. Default is 4.
</td>
</tr><tr>
<td>
`format`
</td>
<td>
(string) format of video, necessary if initializing with path or io object.
</td>
</tr>
</table>



## Methods

<h3 id="encode"><code>encode</code></h3>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/data_types.py">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>encode() -> None
</code></pre>








<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Class Variables</h2></th></tr>

<tr>
<td>
EXTS<a id="EXTS"></a>
</td>
<td>

</td>
</tr><tr>
<td>
artifact_type<a id="artifact_type"></a>
</td>
<td>
`'video-file'`
</td>
</tr>
</table>

