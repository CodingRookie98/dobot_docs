::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](GetK210CarColorParams.htm "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../CarCamera/SetCameraCalibrationMode.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 9 MagicianGO API \> 9.6 CarCamera \>
:::

::: {#winchm_template_title}
9.6.4 GetCarCameraObj
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: 获取K210识别标记模块信息**

**KeyWords:**

portName: string

angle: int

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetCarCameraObj",
    "params": {
        "portName": "COM4"
    }
}
```

 

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0.5em 0px; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "count" : 2  //返回多少组数据,暂定最大值为5
    "dl_obj" :[
             {
            "x" : 1, //x坐标
            "y" : 1, //Y坐标
            "w" : 1, //物体W宽度
            "h" : 1, //物体H高度
            "id" : 1 //类型
             },
             {
            "x" : 1, //x坐标
            "y" : 1, //Y坐标
            "w" : 1, //物体W宽度
            "h" : 1, //物体H高度
            "id" : 2 //类型
             }
    ]
       
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
