# Import & Export API

[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/__init__.py)

Use the Public API to export or update data that you have saved to W&B.

Before using this API, you'll want to log data from your script — check the [Quickstart](https://github.com/charlesfrye/docs-box/tree/1556da259cd7af093524c310c4c6c9746f69ced3/ref/quickstart.md) for more details.

**Use Cases for the Public API**

* **Export Data**: Pull down a dataframe for custom analysis in a Jupyter Notebook. Once you have explored the data, you can sync your findings by creating a new analysis run and logging results, for example: `wandb.init(job_type="analysis")`
* **Update Existing Runs**: You can update the data logged in association with a W&B run. For example, you might want to update the config of a set of runs to include additional information, like the architecture or a hyperparameter that wasn't originally logged.

See the [Generated Reference Docs](https://github.com/charlesfrye/docs-box/tree/1556da259cd7af093524c310c4c6c9746f69ced3/ref/ref/public-api/README.md) for details on available functions.

## Classes

[`class Api`](api.md): Used for querying the wandb server.

[`class Artifact`](artifact.md): An artifact that has been logged, including all its attributes, links to the runs

[`class File`](file.md): File is a class associated with a file saved by wandb.

[`class Files`](files.md): Files is an iterable collection of `File` objects.

[`class Project`](project.md): A project is a namespace for runs

[`class Projects`](projects.md): An iterable collection of `Project` objects.

[`class Run`](run.md): A single run associated with an entity and project.

[`class Runs`](runs.md): An iterable collection of runs associated with a project and optional filter.

[`class Sweep`](sweep.md): A set of runs associated with a sweep

