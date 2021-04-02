# save



[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/3a0def97afe1def2b1a59786b4f0bbcac3f5dc4c/wandb/sdk/wandb_run.py#L1027-L1116)




Ensure all files matching *glob_str* are synced to wandb with the policy specified.

<pre><code>save(
    glob_str: Optional[str] = None,
    base_path: Optional[str] = None,
    policy: str = &#x27;live&#x27;
) -> Union[bool, List[str]]</code></pre>





<!-- Tabular view -->
<table>
<tr><th>Arguments</th></tr>
<tr>
<td>
glob_str (string): a relative or absolute path to a unix glob or regular
path.  If this isn't specified the method is a noop.
base_path (string): the base path to run the glob relative to
policy (string): on of <code>live</code>, <code>now</code>, or <code>end</code>
- live: upload the file as it changes, overwriting the previous version
- now: upload the file once now
- end: only upload file when the run ends
</td>
</tr>

</table>

