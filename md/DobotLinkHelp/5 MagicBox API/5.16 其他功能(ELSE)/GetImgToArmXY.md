::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](../../MagicianGO/MagicBox/GetStopPointState.htm "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../../DebuggerLite/Main.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 9 MagicianGO API \> 9.8 其他（GO相关） \>
:::

::: {#winchm_template_title}
9.8.4 GetImgToArmXY
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**图像坐标转机械臂坐标**

 

请求参数 params

  ----------------- --------- ----------- -----------------
   字段             类型      是否必填    说明 
   portName          string    是          通信端口
   imgX              float     是          图像坐标X
   imgY              float     是          图像坐标Y
   needTranxy        int       是          是否需要转换XY
   suckApriltag      int       是          抓取二维码
   apriltagHeight    int       是          抓取二维码高度
  ----------------- --------- ----------- -----------------

 

 

响应参数 result

  --------- -------- ----------- --------------------------------------
   字段     类型     是否必填    说明 
   armX      float    是          机械臂坐标X
   armY      float    是          机械臂坐标Y
   okflag    int      是         是否运行成功（1：成功，其它：失败） 
  --------- -------- ----------- --------------------------------------

 

 

**KeyWords:**

portName: string

imgX: float, 图像坐标X

imgY: float, 图像坐标Y

needTranxy: int,是否需要转换XY

suckApriltag: int,抓取二维码

apriltagHeight: int,抓取二维码高度

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetImgToArmXY",
    "params": {
        "portName": "COM4",
        "imgX": 50.1,
        "imgY": 100.8,
        "needTranxy": 1,
        "suckApriltag": 1,
        "apriltagHeight":10
    }
}
```

 

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "armX": 263.8121643066406,
        "armY": -64.5769271850586,
        "okflag": 1
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

\

------------------------------------------------------------------------

\
This file is decompiled from a .CHM file\
by an UNREGISTERED version of Easy CHM.\
You can download Easy CHM at :
[http://www.eTextWizard.com](http://www.etextwizard.com/){target="_blank"}\
\
