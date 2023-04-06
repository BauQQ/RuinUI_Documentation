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
#### Find the player if they exist

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Player name |

 Returns **Player name (string)** or **Boolean**
 

 <br />


```
  Player.Class(name);
```
#### Return the class of the player if they exist

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | Player name - can be null |

 Returns **Class object**
 
| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `key` | `int` | Class key |
| `type` | `string` | Class name |

<br />

```
  Player.Level(name);
```
#### Return the level of the player if they exist


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | Player name - can be null |

Returns **Player Level (Int)**



<br />

```
  Player.Faction(name);
```
#### Return the faction of a player if they exist


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | Player name - can be null |

Returns **Faction object**

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `key` | `int` | Faction key |
| `faction` | `string` | Faction name |

<br />

```
  Player.Name();
```
#### Return the name of the player/character currently on

Returns **Player name (string)**

<br />


```
  Player.IsBlocked(name);
```
#### Have you blocked this player


| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Player name |

Returns **Boolean**
