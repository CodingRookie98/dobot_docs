::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](QueuedCmdStartDownload.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetQueuedCmdCurrentIndex.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 5 MagicBox API \> 5.3 队列控制指令(QUEUE) \>
:::

::: {#winchm_template_title}
5.3.5 QueuedCmdStopDownload
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
[**完成指令队列下载**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

 

<div>

请求参数 params

</div>

<div>

 

</div>

<div>

  ----------- --------- ----------- -----------
   字段       类型      是否必填    说明 
   portName   string    是           通信端口
  ----------- --------- ----------- -----------

</div>

<div>

 

</div>

<div>

 

</div>

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

<div>

 

</div>

 

 

**KeyWords:**

portName: string

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.QueuedCmdStopDownload",
    "params": {
        "portName": "COM4"
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
