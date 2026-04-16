::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](GetJOGCommonParams.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../ptp/PTP-tips.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.9 点动功能(JOG) \>
:::

::: {#winchm_template_title}
4.9.7 SetJOGCmd
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
[执行点动功能]{style="FONT-SIZE: 14.05pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

 

请求参数 params

  ----------- --------- ------------ -----------------------------------------------------------------------------------------------------------------------------------------------------------
   字段        类型      是否必填     说明 
   portName    string    是           通信端口
   isJoint     bool      是           点动方式 （false：坐标轴点动 true：关节点动）
   cmd         int       是           点动命令（ 0：停止执行、1：x正方向运行、2：x反方向运行、3：y正反向运行、4：y反方向运行、5：z正方向运行、6：z反方向运行、7：r正方向运行、8：r反方向运行）
   isQueued    bool      否           队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ------------ -----------------------------------------------------------------------------------------------------------------------------------------------------------

 

<div>

<div>

响应参数 result

</div>

<div>

 

</div>

<div>

  --------- ------- ----------- ----------------------------------------------
   字段     类型    是否必填    说明 
   result   bool    是           响应结果（true：操作成功，false：操作失败）
  --------- ------- ----------- ----------------------------------------------

</div>

</div>

 

**KeyWords:**

portName: string

isJoint: bool

cmd: int (0:stop X:1,2 Y:3,4 Z:5,6 R:7,8)

\*isQueued: bool (default:false)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetJOGCmd",
    "params": {
        "portName": "COM4",
        "isJoint": false,
        "cmd": 2,
        "isQueued": false
    }
}
```

 

OUTPUT：

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
