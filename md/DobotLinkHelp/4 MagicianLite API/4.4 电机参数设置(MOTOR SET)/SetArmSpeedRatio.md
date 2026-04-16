::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](../queue/GetQueuedCmdLeftSpace.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetArmSpeedRatio.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.4 电机参数设置(MOTOR SET) \>
:::

::: {#winchm_template_title}
4.4.1 SetArmSpeedRatio
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**设置机械臂速度**

 

请求参数 params

 

  ----------- --------- ----------- -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   字段        类型      是否必填    说明
   portName    string    是          通信端口
   type        int       是          运动类型（0是点动速度，1是点到点的运动速度）
   value       int       是         [ 机械臂的速度值 (0\~100 unit:%)]{style="FONT-SIZE: 14px; FONT-FAMILY: \"Microsoft YaHei\", \"Segoe UI\", system-ui, Roboto, \"Droid Sans\", \"Helvetica Neue\", sans-serif, Tahoma, \"Segoe UI SymbolMyanmar Text\", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"}
   isQueued    bool      是          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行）
  ----------- --------- ----------- -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 

<div>

响应参数 result

</div>

<div>

 

</div>

<div>

  --------- ------- ----------- --------------------------------------------
   字段     类型    是否必填    说明 
   result   bool    是           响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

</div>

 

 

**KeyWords:**

portName: string

type : int (0:JOG 1:PTP)

value: int (0\~100 unit:%)

\*isQueued: bool (default:false)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetArmSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1,
        "value": 50,
        "isQueued": false
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
