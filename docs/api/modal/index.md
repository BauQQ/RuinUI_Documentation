## Modal Api Reference

```
  Modal.Create(data, innerHtml, mainMenu);
```
#### Create and append a new modal-window to the game

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `data` | `Object` | **Required**. Data object, see example below* |
| `innerHtml` | `Object` | **Required**. Data object, see example below** |
| `mainMenu` | `Object` | **Default false**. Set to true if your modal needs a mainMenu element |

Returns **Boolean**

<br />

```
  Modal.Exist(name);
```
#### Check if the modal already exist

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `String` | **Required**. Name to check |

Returns **Boolean**

<br />


#### Elements

| Parameter | Type |
| :------------------------- | :------- |
| `settingMenuButton` | `string` | 
| `tickbox` | `string` | 
| `textbox` | `string` | 
| `inputcolor` | `string` | 
| `ntextbox` | `string` | 
| `decimaltextbox` | `string` | 
| `dnumberbox` | `string` | 
| `hiddeninput` | `string` | 
| `textboxR` | `string` | 
| `numberbox` | `string` | 
| `settingTitle` | `string` | 
| `description` | `string` | 
| `spacer` | `string` | 
| `textarea` | `string` | 
| `doubleBuffDivText` | `string` | 
| `doubleBuffDiv` | `string` | 
| `doubleBuffDivItem` | `string` | 
| `doubleBuffDivImg` | `string` | 
| `buttonL` | `string` | 
| `buttonR` | `string` | 
| `auraButton` | `string` | 
| `bossnexttimer` | `string` | 
| `mainMenuButton` | `string` | 
| `windowPanel` | `string` | 
| `smallPanel` | `string` | 
| `ahfilterbox` | `string` | 
| `sdropdown` | `string` | 
| `sdropdownOption` | `string` | 
| `stashAllButton` | `string` | 
| `withdrawAllButton` | `string` | 
| `menuMouseOverTextBar` | `string` | 
| `textbox_default` | `string` | 
| `basic_itemstat_div` | `string` | 
| `nextboss_i_button` | `string` | 
| `itemization_i_button` | `string` | 
| `stopwatch_i_button` | `string` | 
| `gm_chat_inject` | `string` | 
| `log_chat_inject` | `string` | 
| `normal_chat_inject` | `string` | 
| `dropdownEntry` | `string` | 
| `settingBasePanel` | `string` | 
| `fllistList` | `string` | 
| `fllistitem` | `string` | 
| `fllistmenuDot` | `string` | 
| `fllistButton` | `string` | 
| `blankDiv` | `string` | 
| `contextMenuElement` | `string` | 
| `divWithAction` | `string` | 
| `chatWindowPanel` | `string` | 
| `chatInput` | `string` | 
| `blankUl` | `string` | 
| `blankLi` | `string` | 
| `blankinput` | `string` | 
| `blanksection` | `string` | 
| `blankChatArticle` | `string` | 
| `blankrangeSlider` | `string` | 
| `colorrangeslider` | `string` | 
| `versionblock` | `string` | 
| `closebtn` | `string` | 
| `topLeftElem` | `string` | 
| `customcssInput` | `string` | 
| `customjsInput` | `string` | 
| `emptyWindow` | `string` | 

<br />


#### Data, Data Object*


```js
const buildData = {
    name : "Party Signups",
    element : "mainMenuButton",
    id : "syspartysign",
    cls : "r2_syspartysign",
    nx: "party_signup",
    base : "windowPanel",
    close: Classes.closefeature,
    internal : "innerPartySignup",
    btn : "U",
    settings : {
        key : "partysignupkey",
        hotkey : "u",
        description: "Party Signup hotkey"
    },
    position : {
        top: 150,
        left: 150
    },
    modable : true,
    size:{
        width:0,
        height:0
    },
    resize:true
}
```

<br />


#### InnerHtml, Data Object**

```js
{
    html:your_inner_html
}

```


<br />

#### Modal Example

```js
 const buildData = {
    name : "Test",
    element : "mainMenuButton",
    id : "systest",
    cls : "r2_test",
    nx: "test_signup",
    base : "windowPanel",
    close: Classes.closefeature,
    internal : "emptyWindow",
    btn : "T",
    settings : {
        key : "partysignupkey",
        hotkey : "t",
        description: "Party Signup hotkey"
    },
    position : {
        top: 150,
        left: 150
    },
    modable : true,
    size:{
        width:0,
        height:0
    },
    resize:true
}

let innerHtml = '<div class="btn r2_test_button">Click Me</div> ';

(async() => {  
    if(await Modal.Create(buildData , {html:innerHtml},  false)){
        UI.Delegate(`#${buildData.cls}`, "click", '.r2_test_button', function(){
            console.log(test);
        });
    }
})();

```