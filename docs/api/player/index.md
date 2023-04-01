## Player Api Reference


```
  Player.Has(name);
```
#### Has the player already been pulled from the api


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Player name |

Returns **Boolean**



<br />


```
  Player.Find(name);
```
#### Pull the player from API

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Player name |

 Returns **Player object**
 
 
 <br />


```
  Player.Class(name);
```
#### Pull the player from API

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Player name |

 Returns **Class object**
 
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `key` | `int` | Class key |
| `type` | `string` | Class name |
