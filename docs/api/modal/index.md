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

| Parameter | Type | html                |
| :------------------------- | :------- | :------------------------- |
| `settingMenuButton` | `string` | `<div class="choice" data-key="%key%">%text%</div>` |  
| `tickbox` | `string` | `<div class="btn checkbox %cls%"></div>` |  
| `textbox` | `string` | `<input type="text" class="%cls%" value="%value%">` |  
| `inputcolor` | `string` | `<input type="color" class="%cls%" value="%value%" hex>` |  
| `ntextbox` | `string` | `<input type="number" class="%cls%" value="%value%">` |  
| `decimaltextbox` | `string` | `<input type="number" step="any" class="%cls%" value="%value%">` |  
| `dnumberbox` | `string` | `<input type="number" step=".01"class="%cls%" value="%value%">` |  
| `hiddeninput` | `string` | `<input type="hidden" %a% class="hidden_input_%n%">` |  
| `textboxR` | `string` | `<div></div><input type="text" class="settings_input_%n%">` |  
| `numberbox` | `string` | `<input type="number" %a% class="nbox_%c%" value="%v%">` |  
| `settingTitle` | `string` | `<div class="divruindiv %cls%">%text%</div>` |  
| `description` | `string` | `<br><small class="textgrey">%text%</small>` |  
| `spacer` | `string` | `<div class="textprimary %cls%">%text%</div><div></div>` |  
| `textarea` | `string` | `<textarea class="settings_textarea_%identifier%" %action% rows="4" cols="50"></textarea>` |  
| `doubleBuffDivText` | `string` | `<div class="textsystem %cls%">ON</div><div class="texterror %clsX%">OFF</div>` |  
| `doubleBuffDiv` | `string` | `<div id="%id%" class="%cls% scrollbar " data-array-location="%array_location%" data-array-type="%array_type%" >%content%</div>` |  
| `doubleBuffDivItem` | `string` | `<div id="%id%" class="buff_item %cls%">%text%</div>` |  
| `doubleBuffDivImg` | `string` | `<img src="%src%" class="buff_item_img %cls%" />` |  
| `buttonL` | `string` | `<div class="btn blue" data-action="%action%">%text%</div><div></div>` |  
| `buttonR` | `string` | `<div></div><div class="btn blue" style="text-align:center;" data-action="%action%">%text%</div>` |  
| `auraButton` | `string` | `<div>%data%</div><div class="btn blue" style="text-align:center;" data-action="%action%">%text%</div>` |  
| `bossnexttimer` | `string` | `<div data-action="%action%">%text%</div>` |  
| `mainMenuButton` | `string` | `<div id="%id%" class="btn border black" style="width: 16px;text-align: center;">%text%</div>` |  
| `windowPanel` | `string` | `<div id="%id%" class="%cls% window panel-black cwindow" data-cl="%n%" style="display:none;"><div class="titleframe titleframe_custom"><div class="textprimary title title_custom"><div name="title">%text%</div></div><img src="/assets/ui/icons/cross.svg?v=35201089" class="btn black svgicon %close%" data-feaureid=""></div><div class="slot" style=""><div class="wrapper">%html%</div></div></div>` |  
| `smallPanel` | `string` | `<small class="marg-top bar btn black grey svelte-1apx3f3 %c%"><div class="textgreen"></div></small>` |  
| `ahfilterbox` | `string` | `<input type="text" %a% class="ah_input_%n%">` |  
| `sdropdown` | `string` | `<select class="%cls%" %action%>%html%</select>` |  
| `sdropdownOption` | `string` | `<option value="%value%" %selected%>%text%</option>` |  
| `stashAllButton` | `string` | `<div class="navbtn btn grey gold depositAll"><img class="svgicon" src="/assets/ui/icons/deposit.svg?v=4597824"><span>A</span></div>` |  
| `withdrawAllButton` | `string` | `<div class="navbtn btn grey gold withdrawAll"><img class="svgicon" src="/assets/ui/icons/withdraw.svg?v=4597824"><span>A</span></div>` |  
| `menuMouseOverTextBar` | `string` | `<div class="btn border grey">%t%</div>` |  
| `textbox_default` | `string` | `<input type="text" %a% class="txtbox_%c%">` |  
| `basic_itemstat_div` | `string` | `<div class="%cls% svelte-e3ao5j">%text%</div>` |  
| `nextboss_i_button` | `string` | `<div class="grid buttons marg-top" style="grid-template-columns:3fr 1fr;">%html%</div>` |  
| `itemization_i_button` | `string` | `<div class="grid buttons marg-top" style=""><input type="text" class="%cls%" value=""></div><div class="grid buttons marg-top" style=""><div data-do="imtsearch" style="text-align:center;" class="btn grey imtsearch" data-action="%action%">Search</div></div>` |  
| `stopwatch_i_button` | `string` | `<div class="grid buttons marg-top" style="grid-template-columns: 3fr 1fr 1fr;"><div class="btn disabled cptnum" style="color: white;">00:00:00</div><div data-do="start" class="btn grey cptstart" data-action="%action%">Start</div><div data-do="reset" class="btn grey cptreset" data-action="%action2%">Reset</div></div>` |  
| `gm_chat_inject` | `string` | `<article class="line svelte-1jc1d13 %c%"><div class="linewrap svelte-1jc1d13"><span class="time svelte-1jc1d13">%t%</span><span class="textsub content svelte-1jc1d13"><span class="capitalize channel svelte-1jc1d13">%n%</span> </span><span class="textsub svelte-1jc1d13">%td%</span></div></article>` |  
| `log_chat_inject` | `string` | `<article class="line svelte-1jc1d13 %c%"><div class="linewrap svelte-1jc1d13"><span class="time svelte-1jc1d13">%t%</span><span class="textlog content svelte-1jc1d13"><span class="capitalize channel svelte-1jc1d13">%n%</span> </span><span class="textlog svelte-1jc1d13">%td%</span></div></article>` |  
| `normal_chat_inject` | `string` | `<article class="line svelte-1jc1d13 %c%"><div class="linewrap svelte-1jc1d13"><span class="time svelte-1jc1d13">%t%</span><span class="textglobal content svelte-1jc1d13"><span class="capitalize channel svelte-1jc1d13">global</span> <span class="sender svelte-1jc1d13"><span class="name textf0 svelte-erbdzy">%n%</span></span></span><span class="textglobal svelte-1jc1d13">%td%</span></div></article>` |  
| `dropdownEntry` | `string` | `<div class="choice %cls%" %action%>%html%</div>` |  
| `settingBasePanel` | `string` | `<div data-panel="%panel%" class="menu scrollbar panel-black %cls%" style="display:none;"><h3 class="textprimary">%text%</h3><div class="settings">%html%</div></div>` |  
| `fllistList` | `string` | `<div class="%c%_list"><ul>%td%</ul></div>` |  
| `fllistitem` | `string` | `<li><div class="dotSquareList"><span class="dot %c%"></span></div><span class="%c2%" data-name="%n%">%t%</span></li>` |  
| `fllistmenuDot` | `string` | `<div class="dotSquare"><span class="dot %c%"></span></div>` |  
| `fllistButton` | `string` | `<div class="btn btn_%c%" %a%>%t%</div>` |  
| `blankDiv` | `string` | `<div class="%c%">%td%</div>` |  
| `contextMenuElement` | `string` | `<div class="panel context border grey %c%">%td%</div>` |  
| `divWithAction` | `string` | `<div class="%c%" %a%>%t%</div>` |  
| `chatWindowPanel` | `string` | `<div class="cl_chat" data-cl="%c%" style="display:block;"><div class="titleframe titleframe_custom">%td%</div><div class="slot %sl%" style="">%td2%</div>%td3%</div>` |  
| `chatInput` | `string` | `<div %s% class="%c%">%td%</div>` |  
| `blankUl` | `string` | `<ul class="%c%" %a%>%td%</ul>` |  
| `blankLi` | `string` | `<li class="%c%" %a%>%t%</li>` |  
| `blankinput` | `string` | `<input class="%c%" type="%t%" %a%>` |  
| `blanksection` | `string` | `<section class="%c%">%td%</section>` |  
| `blankChatArticle` | `string` | `<article class="line svelte-1jc1d13" %a%><div class="linewrap svelte-1jc1d13"><span class="time svelte-1jc1d13">%ti%</span><span class="%c% content svelte-1jc1d13"><span class="capitalize channel svelte-1jc1d13">%td2%</span> <span class="sender svelte-1jc1d13"><span class="textwhite"><img class="icon svelte-erbdzy" src="%cls%">%lvl%</span><span class="name %fc% svelte-erbdzy">%name%</span></span></span><span class="%c2% svelte-1jc1d13">%m%</span></div></article>` |  
| `blankrangeSlider` | `string` | `<input type="range" class="%c%" %a%>` |  
| `colorrangeslider` | `string` | `<input type="range" value="%value%" min="0" max="99" step="1" class="%cls%" %a%>` |  
| `versionblock` | `string` | `<div class="l-corner-lr container svelte-1axz35 versiondiv">%modname%: %version% - By %by%</div>` |  
| `closebtn` | `string` | `<img src="/assets/ui/icons/cross.svg?v=35201089" class="btn black svgicon %close%">` |  
| `topLeftElem` | `string` | `<div class="btn border grey %cls%">%content%</div>` |  
| `customcssInput` | `string` | `<textarea class="settings_textarea_%identifier% scrollbar" %action% rows="%rows%" cols="%cols%"></textarea>` |  
| `customjsInput` | `string` | `<div class="customJsGridModifier"><textarea class="settings_textarea_%identifier% scrollbar" %action% rows="%rows%" cols="%cols%"></textarea></div>` |  
| `innerPartySignup` | `string` | `<table class="marg-top panel-black playerlist">%html%</table>` |  
| `emptyWindow` | `string` | `<div class="emptyWindowClass">%html%</div>` |  

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