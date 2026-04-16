::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](QueuedCmdStopDownload.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetQueuedCmdLeftSpace.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.3 队列控制指令(QUEUE) \>
:::

::: {#winchm_template_title}
4.3.6 GetQueuedCmdCurrentIndex
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
 

<div>

[**获取指令队列索引**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

 

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

+-----------------+-----------------+-----------------+-----------------+
|  字段           | 类型            | 是否必填        | 说明            |
+-----------------+-----------------+-----------------+-----------------+
|  queuedCmdIndex | int             | 是              | ::: {s          |
|                 |                 |                 | tyle="FONT-SIZE |
|                 |                 |                 | : medium; WHITE |
|                 |                 |                 | -SPACE: normal; |
|                 |                 |                 |  WORD-SPACING:  |
|                 |                 |                 | 0px; TEXT-TRANS |
|                 |                 |                 | FORM: none; FON |
|                 |                 |                 | T-WEIGHT: 400;  |
|                 |                 |                 | COLOR: rgb(0,0, |
|                 |                 |                 | 0); FONT-STYLE: |
|                 |                 |                 |  normal; ORPHAN |
|                 |                 |                 | S: 2; WIDOWS: 2 |
|                 |                 |                 | ; LETTER-SPACIN |
|                 |                 |                 | G: normal; TEXT |
|                 |                 |                 | -INDENT: 0px; f |
|                 |                 |                 | ont-variant-lig |
|                 |                 |                 | atures: normal; |
|                 |                 |                 |  font-variant-c |
|                 |                 |                 | aps: normal; -w |
|                 |                 |                 | ebkit-text-stro |
|                 |                 |                 | ke-width: 0px;  |
|                 |                 |                 | text-decoration |
|                 |                 |                 | -style: initial |
|                 |                 |                 | ; text-decorati |
|                 |                 |                 | on-color: initi |
|                 |                 |                 | al; text-decora |
|                 |                 |                 | tion-thickness: |
|                 |                 |                 |  initial" ksdoc |
|                 |                 |                 | clipboard="ksDo |
|                 |                 |                 | cClipboardId:'{ |
|                 |                 |                 | 10364193-f0ce-b |
|                 |                 |                 | b57-d0df-1e7bec |
|                 |                 |                 | 861d33-47399316 |
|                 |                 |                 | 516}';from:'wps |
|                 |                 |                 | ';priorityForma |
|                 |                 |                 | t:'Kingsoft WPS |
|                 |                 |                 |  9.0 Format';mi |
|                 |                 |                 | metypes:'Kingso |
|                 |                 |                 | ft WPS 9.0 Form |
|                 |                 |                 | at;text/html'"} |
|                 |                 |                 | [[]{style="F    |
|                 |                 |                 | ONT-SIZE: 10.5p |
|                 |                 |                 | t; FONT-FAMILY: |
|                 |                 |                 |  Calibri"}]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 10.5pt; FONT-FA |
|                 |                 |                 | MILY: Calibri"} |
|                 |                 |                 |                 |
|                 |                 |                 | [队列命令       |
|                 |                 |                 | 索引]{style="FO |
|                 |                 |                 | NT-SIZE: 10.5pt |
|                 |                 |                 | ; FONT-FAMILY:  |
|                 |                 |                 | Calibri"}[]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 10.5pt; FONT-FA |
|                 |                 |                 | MILY: Calibri"} |
|                 |                 |                 | :::             |
+-----------------+-----------------+-----------------+-----------------+

</div>

 

 

**KeyWords:**

portName: string

queuedCmdIndex: int

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetQueuedCmdCurrentIndex",
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
        "queuedCmdIndex": 56
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
