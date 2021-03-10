description: Wandb is a library to help track machine learning experiments.
robots: noindex

# Module: ref

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">

</table>

<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/library/__init__.py">View source</a>



Wandb is a library to help track machine learning experiments.


For more information on wandb see https://docs.wandb.com.

The most commonly used functions/objects are:
- wandb.init — initialize a new run at the top of your training script
- wandb.config — track hyperparameters
- wandb.log — log metrics over time within your training loop
- wandb.save — save files in association with your run, like model weights
- wandb.restore — restore the state of your code when you ran a given run

For examples usage, see github.com/wandb/examples

## Classes

[`class Api`](./ref/Api.md): Used for querying the wandb server.

[`class Audio`](./ref/Audio.md): Wandb class for audio clips.

[`class Graph`](./ref/Graph.md): Wandb class for graphs

[`class Histogram`](./ref/Histogram.md): wandb class for histograms.

[`class Html`](./ref/Html.md): Wandb class for arbitrary html

[`class Image`](./ref/Image.md): Wandb class for images.

[`class Molecule`](./ref/Molecule.md): Wandb class for Molecular data

[`class Object3D`](./ref/Object3D.md): Wandb class for 3D point clouds.

[`class Plotly`](./ref/Plotly.md): Wandb class for plotly plots.

[`class Table`](./ref/Table.md): This is a table designed to display sets of records.

[`class Video`](./ref/Video.md): Wandb representation of video.

## Functions

[`agent(...)`](./ref/agent.md): Generic agent entrypoint, used for CLI or jupyter.

[`config(...)`](./ref/config.md): Config object

[`init(...)`](./ref/init.md): Start a new tracked run with `wandb.init()`.

[`join(...)`](./ref/join.md): Marks a run as finished, and finishes uploading all data.

[`log(...)`](./ref/log.md): Log a dict to the global run's history.

[`save(...)`](./ref/save.md): Ensure all files matching *glob_str* are synced to wandb with the policy specified.

[`setup(...)`](./ref/setup.md)

[`summary(...)`](./ref/summary.md): Summary tracks single values for each run. By default, summary is set to the

[`sweep(...)`](./ref/sweep.md)



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Other Members</h2></th></tr>

<tr>
<td>
__version__<a id="__version__"></a>
</td>
<td>
`'0.10.22'`
</td>
</tr>
</table>

