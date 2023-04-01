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


```
  Utility.Ucwords(sentence);
```
#### Capitalize first letter of all words on the string

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `sentence` | `string` | **Required**. String to modify |

 Returns **String**
 
| Type     | Description                |
| :------- | :------------------------- |
| `String` | Result of string modification |

<br />

```
  Utility.TableIsTrue(table);
```
#### Check if all values in a 1-dimensinal table is true

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `table` | `object` | **Required**. Object to check |

 Returns **Boolean**

<br />

```
  Utility.ToMilliseconds(hour, minute, second);
```
#### How many miliseconds is the time input

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `hour` | `int` | **Required**. Hours to be added up |
| `minute` | `int` | **Required**. Minutes to be added up |
| `second` | `int` | **Required**. Seconds to be added up |

 Returns **Int**
 
| Type     | Description                |
| :------- | :------------------------- |
| `int` | Result of input in milliseconds |

<br />


```
  Utility.ToMinutes(ms);
```
#### How many minutes is the miliseconds input

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `ms` | `int` | **Required**. Miliseconds to be calculated |

 Returns **Int**
 
| Type     | Description                |
| :------- | :------------------------- |
| `int` | Result of input in minutes |

<br />


```
  Utility.Clone(obj);
```
#### Get a fresh clone of the object

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `obj` | `object` | **Required**. Object to be cloned |

 Returns **Object**
 
| Type     | Description                |
| :------- | :------------------------- |
| `object` | Result of cloning |

<br />

```
  Utility.FindPropertyCaseInsensitive(obj, key);
```
#### Find a property in the object by key

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `obj` | `object` | **Required**. Object to be searched |
| `key` | `string` | **Required**. Key of the property to be found |

 Returns **Object or Null**
 
| Type     | Description                |
| :------- | :------------------------- |
| `object` | Result of search |

<br />


```
  Utility.GetTime();
```
#### Get Ruin UI Base time

Returns **Date Object**

| Type     | Description                |
| :-------- | :------------------------- |
| `Date Object` | Date time Object for Ruin UI Basetime |

<br />


```
  Utility.ToLocalTime(stamp);
```
#### Timestamp to users localtime

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `stamp` | `int` | **Required**. Timestamp in seconds |

 Returns **Date Object**
 
| Type     | Description                |
| :------- | :------------------------- |
| `Date Object` | Result of creating a date from input seconds |

<br />


```
  Utility.GetKeybinds();
```
#### Get keybinds from the datastorage for the game

Returns **Object**

| Type     | Description                |
| :-------- | :------------------------- |
| `Object` | Object contains all the keybinds |

<br />

```
  Utility.isEmpty(string);
```
#### Check if the string is empty

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `string` | `string` | **Required**. String to check |

 Returns **Boolean**

<br />