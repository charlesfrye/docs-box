description: Marks a run as finished, and finishes uploading all data.
robots: noindex

# liberry.join

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/sdk/wandb_run.py">View source</a>



Marks a run as finished, and finishes uploading all data.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>liberry.join(
    exit_code: int = None
) -> None
</code></pre>



<!-- Placeholder for "Used in" -->

This is used when creating multiple runs in the same process.
We automatically call this method when your script exits.