::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetDIValue.html "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetVisionCoordinate.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 8 MagicianPro API \> 8.11 运动指令GO \>
:::

::: {#winchm_template_title}
8.11.1 GO
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**KeyWords:**

portName: string

data: object

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetCRRunTo",
    "params": {
        "portName": "192.168.1.6",
        "data": {
             "value": true/false, false是停止运动，true是开始运动     
             "x": 0,
             "y": 0,
             "z": 0,
             "a": 0,
             "b": 0,
             "c": 0,
             "r": -1,
             "d": -1,
             "n": -1,
             "mode" : "go"/"move"/"jump" ,
             "cfg": -1,
             "tool": 0,
             "user": 0
        }
    }
}
```
:::
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::
