::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetCPParams.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetCPCmd.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.13 连续轨迹运动(CP) \>
:::

::: {#winchm_template_title}
4.13.2 GetCPParams
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
[**获取连续运动轨迹参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

 

请求参数 params

  ----------- --------- ----------- -----------
   字段        类型     是否必填    说明 
   portName    string    是          通信端口
  ----------- --------- ----------- -----------

 

 

<div>

响应参数 result

</div>

 

  ------------------ --------- ------------ --------------------------------------------------------------------------------------------------------------------------
   字段               类型      是否必填      说明 
   portName           string    是           通信端口
   targetAcc          float     是           [规划加速度最大值]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
   junctionVel        float     是            [ 拐角加速度最大值]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; 
                                            COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
   isRealTimeTrack    bool      是           是否开启实时模式（ true: 是 false: 否）
   acc                float     否           [实际加速度最大值，非实时模式下使用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
   period             float     否           [插补周期，实时模式下使用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  ------------------ --------- ------------ --------------------------------------------------------------------------------------------------------------------------

 

**KeyWords:**

portName: string

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

\*acc: float(isRealTimeTrack = false)

\*period: float(isRealTimeTrack = true)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetCPParams",
    "params": {
        "portName": "COM4"
    }
}
```

 

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0.5em 0px; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100
    }
}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "isRealTimeTrack": true,
        "junctionVel": 100,
        "period": 20,
        "targetAcc": 200
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
