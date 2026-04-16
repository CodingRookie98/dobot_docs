::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](GetDeviceSN.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetDeviceVersion.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 5 MagicBox API \> 5.2 设备信息(DEVICE) \>
:::

::: {#winchm_template_title}
5.2.3 GetDeviceName
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**获取设备名称**

 

请求参数 params

 

  ----------- --------- ----------- -----------
   字段       类型      是否必填    说明 
   portName   string    是           通信端口
  ----------- --------- ----------- -----------

 

<div>

响应参数 result

</div>

<div>

 

</div>

<div>

 

</div>

<div>

  ------------- -------- ----------- -----------
   字段         类型     是否必填    说明 
   deviceName   string   是           设备名称
  ------------- -------- ----------- -----------

</div>

 

 

**KeyWords:**

portName: string

deviceName: string

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetDeviceName",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",

    "result": {
        "deviceName": "Dobot123"
       }
}
```

` `{.language-json
style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: visible; WORD-WRAP: normal; BORDER-TOP: 0px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BORDER-RIGHT: 0px; BACKGROUND: none transparent scroll repeat 0% 0%; WHITE-SPACE: pre; WORD-SPACING: normal; BORDER-BOTTOM: 0px; WORD-BREAK: normal; COLOR: black; PADDING-BOTTOM: 0px; TEXT-ALIGN: left; PADDING-TOP: 0px; PADDING-LEFT: 0px; BORDER-LEFT: 0px; MARGIN: 0px; DISPLAY: inline; PADDING-RIGHT: 0px; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
:::
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::

\

------------------------------------------------------------------------

\
This file is decompiled from a .CHM file\
by an UNREGISTERED version of Easy CHM.\
You can download Easy CHM at :
[http://www.eTextWizard.com](http://www.etextwizard.com/){target="_blank"}\
\
