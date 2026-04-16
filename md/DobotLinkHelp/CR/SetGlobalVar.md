::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetApiUpdate.htm "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetGlobalVar.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 7 CR API \> [7.25 Other(unknown)](../$$unsavedpage1.htm) \>
:::

::: {#winchm_template_title}
7.25.14 SetGlobalVar
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
功能:

    全局变量的设置

::: {#nstext}
INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetGlobalVar",
    "params": {
        "portName": "192.168.5.1",
  "data":{
   "var1": {
    "globalHold": true, --是否全局保持
    "value": 20 --int类型
   },
   "var2": {
    "globalHold": false, --是否全局保持
    "value": 20.5 --double型
   },
   "var3": {
    "globalHold": true, --是否全局保持
    "value": "string" --string型
   },
   "var4": {
    "globalHold": true, --是否全局保持
    "value": true --bool型
   },
   "var5": {
    "globalHold": true, --是否全局保持
    "value":{ --point示教点
    "armOrientation": [
     -1,
     -1,
     -1,
     0
    ],
    "coordinate": [
     1,
     2,
     3,
     4,
     5,
     6
    ],

    "tool": 0,

    "user": 0

    }

    }

    }


    }

}
```
:::

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{

    "id": 1,

    "jsonrpc": "2.0",
    "result": {"status":true/false}
}
```

\
 
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::
