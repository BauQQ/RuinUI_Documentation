## Character Api Reference

```
  Character.Id();
```
#### Return the current characters id

Returns **Character id**

| Type     | Description                |
| :-------- | :------------------------- |
| `string` | Character id |

<br />



```
  Character.ClassByImage(url);
```
#### Get the class from the class icon image

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `url` | `string` | **Required**. Image url |

Returns **Object**

| Name     | Type     | Description                |
| :-------- | :-------- | :------------------------- |
| `key` | `int` | class id |
| `type` | `string` | Class name |

<br />


```
  Character.IsPartyLead(name);
```
#### Figure out of the player is a partyleader of your party

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Player to check |

Returns **Boolean**

<br />


```
  Character.IsInParty();
```
#### Are you in a party

Returns **Boolean**
<br />