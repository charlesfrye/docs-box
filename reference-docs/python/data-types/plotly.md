# Plotly

[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/sdk/data_types.py#L1983-L2030)

Wandb class for plotly plots.

```text
Plotly(
    val: Union['plotly.Figure', 'matplotlib.artist.Artist']
)
```

| Arguments |  |
| :--- | :--- |
|  `val` |  matplotlib or plotly figure |

## Methods

### `make_plot_media` <a id="make_plot_media"></a>

[View source](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/sdk/data_types.py#L1991-L1999)

```text
@classmethod
make_plot_media(
    val: Union['plotly.Figure', 'matplotlib.artist.Artist']
) -> Union[Image, 'Plotly']
```

| Class Variables |  |
| :--- | :--- |
|  artifact\_type |  `None` |

