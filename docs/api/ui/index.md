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
