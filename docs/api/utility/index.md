## Utility Api Reference

```
  Utility.Time();
```
#### Ask for the current clock

Returns **Clock string**
| Type     | Description                |
| :-------- | :------------------------- |
| `string` | Clock string  `${b}:${c}` |
<br />


```
  Utility.Copy(data);
```
#### Send a string to the clipboard

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `data` | `string` | **Required**. String you want to send to clipboard |

<br />

```
  Utility.Ucfirst(word);
```
#### Make the first letter in a string Capitalized

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `word` | `string` | **Required**. String to modify|

 Returns **String**
 
| Type     | Description                |
| :------- | :------------------------- |
| `String` | Result of string modification |

<br />