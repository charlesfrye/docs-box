# join

<!-- Insert buttons and diff -->




<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/ref/sdk/wandb_run.py">View source</a>



Marks a run as finished, and finishes uploading all data.

<pre><code>join(
    exit_code: int = None
) -> None</code></pre>



<!-- Placeholder for "Used in" -->

This is used when creating multiple runs in the same process.
We automatically call this method when your script exits.