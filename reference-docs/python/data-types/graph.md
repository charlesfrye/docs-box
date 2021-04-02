# Graph

[![](https://www.tensorflow.org/images/GitHub-Mark-32px.png)View source on GitHub](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/data_types.py#L1035-L1193)

Wandb class for graphs

```text
Graph(
    format='keras'
)
```

This class is typically used for saving and diplaying neural net models. It represents the graph as an array of nodes and edges. The nodes can have labels that can be visualized by wandb.

#### Examples:

Import a keras model:

```text
    Graph.from_keras(keras_model)
```

## Methods

### `add_edge` <a id="add_edge"></a>

[View source](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/data_types.py#L1119-L1123)

```text
add_edge(
    from_node, to_node
)
```

### `add_node` <a id="add_node"></a>

[View source](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/data_types.py#L1105-L1117)

```text
add_node(
    node=None, **node_kwargs
)
```

### `from_keras` <a id="from_keras"></a>

[View source](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/data_types.py#L1125-L1154)

```text
@classmethod
from_keras(
    model
)
```

### `pprint` <a id="pprint"></a>

[View source](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/data_types.py#L1099-L1103)

```text
pprint()
```

### `__getitem__` <a id="__getitem__"></a>

[View source](https://www.github.com/wandb/client/tree/7bbc4a4eac8eeb2bf37a62ce519e0de61c67eadf/wandb/data_types.py#L1096-L1097)

```text
__getitem__(
    nid
)
```

| Class Variables |  |
| :--- | :--- |
|  artifact\_type |  `None` |

