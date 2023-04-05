## Inject Api Reference

```
  Inject.AddExecuteOnWindowLoad(window, func);
```
#### Add your own functions to run upon a specific window is opened

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `window` | `string` | **Required**. Key / Name of the window |
| `func` | `function` | **Required**. Function to run |

<br />


```
  Inject.RemoveExecuteOnWindowLoad(window, func);
```
#### Remove the specific function from the execution list

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `window` | `string` | **Required**. Key / Name of the window |
| `func` | `function` | **Required**. Function to run |

<br />


### Window Key List

| Key |
| :----- |
| `character`|
| `clan`
| `interaction`|
| `merchant`|
| `pvp`|
| `request`|
| `skills`|
| `stash`|
| `store / elixir`|
| `trader`|