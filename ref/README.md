# ref

<!-- Insert buttons and diff -->




<a target="_blank" href="https://charlesfrye.gitbook.io/docs-box/ref/__init__.py">View source</a>



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

[`class Api`](./api.md): Used for querying the wandb server.

[`class Audio`](./audio.md): Wandb class for audio clips.

[`class Graph`](./graph.md): Wandb class for graphs

[`class Histogram`](./histogram.md): wandb class for histograms.

[`class Html`](./html.md): Wandb class for arbitrary html

[`class Image`](./image.md): Wandb class for images.

[`class Molecule`](./molecule.md): Wandb class for Molecular data

[`class Object3D`](./object3d.md): Wandb class for 3D point clouds.

[`class Plotly`](./plotly.md): Wandb class for plotly plots.

[`class Table`](./table.md): This is a table designed to display sets of records.

[`class Video`](./video.md): Wandb representation of video.

## Functions

[`agent(...)`](./agent.md): Generic agent entrypoint, used for CLI or jupyter.

[`config(...)`](./config.md): Config object

[`init(...)`](./init.md): Start a new tracked run with `wandb.init()`.

[`join(...)`](./join.md): Marks a run as finished, and finishes uploading all data.

[`log(...)`](./log.md): Log a dict to the global run's history.

[`save(...)`](./save.md): Ensure all files matching *glob_str* are synced to wandb with the policy specified.

[`setup(...)`](./setup.md)

[`summary(...)`](./summary.md): Summary tracks single values for each run. By default, summary is set to the

[`sweep(...)`](./sweep.md)



<!-- Tabular view -->
<table>
<tr><th>Other Members</th></tr>

<tr>
<td>
__version__<a id="__version__"></a>
</td>
<td>
`'0.10.22'`
</td>
</tr>
</table>

