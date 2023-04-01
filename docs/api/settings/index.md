## Settings Api Reference

```
  Settings.Get(name);
```
#### Get set value of a setting by name

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Name of the setting you want |

Returns **Int/String/Boolean**

<br />


```
  Settings.Check(name);
```
#### Check if the setting exist

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Name of the setting |

Returns **Boolean**

<br />