::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetSafeParams.html "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetElecSkinEnable.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 7 CR API \> 7.13 协作机器人安全配置 \>
:::

::: {#winchm_template_title}
7.13.6 SetCollisionDetectParam
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
[安全碰撞设置的万能接口，可以修改添加任意字段]{style="FONT-SIZE: 14px; FONT-FAMILY: \"Microsoft YaHei\", \"Segoe UI\", system-ui, Roboto, \"Droid Sans\", \"Helvetica Neue\", sans-serif, Tahoma, \"Segoe UI Symbol\", \"Myanmar Text\", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"}

[]{style="FONT-SIZE: 14px; FONT-FAMILY: \"Microsoft YaHei\", \"Segoe UI\", system-ui, Roboto, \"Droid Sans\", \"Helvetica Neue\", sans-serif, Tahoma, \"Segoe UI Symbol\", \"Myanmar Text\", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"} 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 0,

    "jsonrpc": "2.0",

    "method": "dobotlink.CR.SetCollisionDetectParam",

    "params": {

         "portName": "192.168.1.6",

          "data": {

            "key": "你要修改的字段名称",

            "value": 任意json数据，可以是值，也可以是 jsonArray, jsonObject
         }
    }
}
```

 

 

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
} 
```
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::
