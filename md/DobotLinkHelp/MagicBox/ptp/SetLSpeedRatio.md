::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetPTPWithLCmd.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetLSpeedRatio.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 5 MagicBox API \> 5.6 滑轨控制(PTP) \>
:::

::: {#winchm_template_title}
5.6.2 SetLSpeedRatio
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
 

<div>

[**设置导轨速度比例**]{style="FONT-SIZE: 9.95pt; FONT-FAMILY: 黑体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

 

请求参数 params

+-----------------+-----------------+-----------------+-----------------+
|  字段           |  类型           |  是否必填       |  说明           |
+-----------------+-----------------+-----------------+-----------------+
|  portName       |  string         |  是             |  通信端口       |
+-----------------+-----------------+-----------------+-----------------+
|  type           |  int            |  是             | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 |  速度参数       |
|                 |                 |                 | 类型（0:JOG、1: |
|                 |                 |                 | PTP）]{style="F |
|                 |                 |                 | ONT-SIZE: 9pt;  |
|                 |                 |                 | FONT-FAMILY: 黑 |
|                 |                 |                 | 体; COLOR: rgb  |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
+-----------------+-----------------+-----------------+-----------------+
|  value          |  int            |  是             |  速度           |
|                 |                 |                 | 比例值（0\~100  |
|                 |                 |                 | unit:%）        |
+-----------------+-----------------+-----------------+-----------------+
|  isQueued       |  bool           |  否             |  队列指令（t    |
|                 |                 |                 | rue：指令排队执 |
|                 |                 |                 | 行，false：打断 |
|                 |                 |                 | 当前执行的任务  |
|                 |                 |                 | ，直接插入执行  |
|                 |                 |                 | ）默认：false   |
+-----------------+-----------------+-----------------+-----------------+

 

 

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

value: int 0\~100(%)

type: int 速度参数类型 0:JOG,1:PTP

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetLSpeedRatio",
    "params": {
        "portName": "COM4",
        "value": 50,
        "type": 0 
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
