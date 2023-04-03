## UI Api Reference

```
  UI.Append(element, html);
```
#### Append some html to a specific element

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `element` | `elementObject` | **Required**. The element to append html to |
| `html` | `string/htmlObject` | **Required**. The html you wan to append |

<br />

```
  UI.Remove(element);
```
#### Remove a specific element

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `element` | `elementObject` | **Required**. The element to remove |

<br />

```
  UI.Empty(element);
```
#### Empty out everything in the element

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `element` | `elementObject` | **Required**. The element to empty |

<br />

```
  UI.AddToMenu(element);
```
#### Add a new button element to the main top menu

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `element` | `elementObject` | **Required**. The button element to add |

<br />

```
  UI.RemoveFromMenu(id);
```
#### Remove a button from the main menu by ID

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id` | `id` | **Required**. The id of the button element to remove |

<br />

```
  UI.AddToMenu(element);
```
#### Add a new button element to the main top menu

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `element` | `elementObject` | **Required**. The button element to add |

<br />

```
  UI.Reload();
```
#### Safe reload of the window/game

<br />

```
  UI.Exist(element);
```
#### Definitively check if the element/object/variable exist

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `element` | `*` | **Required**. What ever you need to check if exist |

<br />

```
  UI.Delegate(parent, trigger, on, action, data = null);
```
#### Setup delegation

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `parent` | `htmlObject/string` | **Required**. The parent element or identifier of element: `.class` / `#id` |
| `trigger` | `string` | **Required**. What that triggers the delegation* |
| `on` | `htmlObject/string` | **Required**. The target element or identifier of element: `.class` / `#id` |
| `action` | `string/function` | **Required**. Function or name of pre-registered function |
| `data` | `*` | **Default NULL** can be anything for passthrough to function|

<br />