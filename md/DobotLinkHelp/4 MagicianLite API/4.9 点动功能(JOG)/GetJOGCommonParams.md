::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetJOGCommonParams.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetJOGCmd.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.9 点动功能(JOG) \>
:::

::: {#winchm_template_title}
4.9.6 GetJOGCommonParams
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
[**获取点动公共参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

 

<div>

请求参数 params

</div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"} 

  ----------- --------- ------------ -----------
   字段        类型      是否必填     说明  
   portName    string    是           通信端口
  ----------- --------- ------------ -----------

 

<div>

响应参数 result

</div>

  -------------------- -------- ------------ -------------------------------------------------------------------------------------------------------------------------------
   字段                  类型    是否必填     说明  
   accelerationRatio   float     是           [ 速度比例，关节点动和坐标轴点动共用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
   velocityRatio       float     是             [ 加速度比例，关节点动和坐标轴点动共用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  -------------------- -------- ------------ -------------------------------------------------------------------------------------------------------------------------------

 

 

 

 

**KeyWords:**

portName: string

velocityRatio: float

accelerationRatio: float

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetJOGCommonParams",
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
        "accelerationRatio": 50,
        "velocityRatio": 100
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
