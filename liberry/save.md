description: Ensure all files matching *glob_str* are synced to wandb with the policy specified.
robots: noindex

# liberry.save

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/wandb_run.py">View source</a>



Ensure all files matching *glob_str* are synced to wandb with the policy specified.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>liberry.save(
    glob_str: Optional[str] = None,
    base_path: Optional[str] = None,
    policy: str = &#x27;live&#x27;
) -> Union[bool, List[str]]
</code></pre>



<!-- Placeholder for "Used in" -->


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Arguments</h2></th></tr>

<tr>
<td>
`glob_str`
</td>
<td>
(string) a relative or absolute path to a unix glob or regular
path.  If this isn't specified the method is a noop.
</td>
</tr><tr>
<td>
`base_path`
</td>
<td>
(string) the base path to run the glob relative to
</td>
</tr><tr>
<td>
`policy`
</td>
<td>
(string) on of `live`, `now`, or `end`
- live: upload the file as it changes, overwriting the previous version
- now: upload the file once now
- end: only upload file when the run ends
</td>
</tr>
</table>

