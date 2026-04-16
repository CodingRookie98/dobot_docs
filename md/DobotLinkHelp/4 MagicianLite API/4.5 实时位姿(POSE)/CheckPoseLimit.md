::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](ResetPose.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../alarm/GetAlarmsState.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.5 实时位姿(POSE) \>
:::

::: {#winchm_template_title}
4.5.3 CheckPoseLimit
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**检查点位限制**

 

请求参数 Params

  ----------- --------- ------------ ------------------------------------------------------------------------------------------------------------------------------
   字段         类型     是否必填     说明 
   portName    string    是           通信端口
   isJoint     bool      是           控制方式（true表示关节坐标系，下面x、y、z、r对应j1、j2、j3、j4，false表示笛卡尔坐标系,x y z r就是x y z r）
   x           float     是           当前x的位置（ [-135°\~135°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
   y           float     是           当前y的位置（ [-5°\~80°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
   z           float     是           当前z的位置（ [-10°\~85°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
   r           float     是           当前r的位置（ [-145°\~145°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
  ----------- --------- ------------ ------------------------------------------------------------------------------------------------------------------------------

 

<div>

响应参数 result

</div>

<div>

 

</div>

<div>

  ------------ ------- ----------- ---------------------------------------------
   字段        类型    是否必填    说明 
   isLimited   bool    是          响应结果（true：操作成功，false：操作失败）
  ------------ ------- ----------- ---------------------------------------------

</div>

 

 

 

**KeyWords:**

portName: string

isJoint: bool (default:false)

x: float

y: float

z: float

r: float

isLimited: bool

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.CheckPoseLimit",
    "params": {
        "portName": "COM4",
        "isJoint": false,
        "x": 100.6,
        "y": 260.0,
        "z": 20.0,
        "r": 0.0
    }
}
```

 

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
 {
     "id": 1,
     "jsonrpc": "2.0",
     "result": {
         "isLimited": false
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
