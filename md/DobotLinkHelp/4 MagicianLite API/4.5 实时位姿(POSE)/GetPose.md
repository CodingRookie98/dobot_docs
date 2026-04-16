::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](../motorset/GetArmSpeedRatio.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](ResetPose.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.5 实时位姿(POSE) \>
:::

::: {#winchm_template_title}
4.5.1 GetPose
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
[**获取实时位置**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

 

<div>

请求参数 params

</div>

<div>

 

</div>

<div>

  ----------- --------- ----------- ----------
   字段       类型      是否必填    说明 
   portName   string    是          通信端口
  ----------- --------- ----------- ----------

</div>

<div>

 

</div>

<div>

 

</div>

<div>

响应参数 result

</div>

<div>

  ------------- --------------- ------------ -------------------------------------------
   字段          类型            是否必填     说明 
   x             float           是           当前x的位置
   y             float           是           当前y的位置
   z             float           是           当前z的位置
   r             float           是           当前r的位置
   jointAngle    array(float)    是           机械臂 4轴（底座、大臂、小臂、末端）角度
  ------------- --------------- ------------ -------------------------------------------

</div>

[]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"} 

**KeyWords:**

portName: string

x: float

y: float

z: float

r: float

jointAngle: array(float)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPose",
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
        "x": 134.01580810546875,
        "y": -5.637601852416992,
        "z": 34.831390380859375,
        "r": -2.4088234901428223,
        "jointAngle": [-2.4088234901428223, 10.456664085388184, 41.771934509277344, 0]
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
