::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](GetMotivationMode.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetMotivateZCmd.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 6 M1 API \> 6.14 激励模式(MOTIVATION) \>
:::

::: {#winchm_template_title}
6.14.3 SetMotivateCmd
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**KeyWords:**

portName: string

q1,q2: float

dq1,dq2: float

ddq1,ddq2: float

\*isQueued: bool (default:true)

\*isWaitForFinish: bool (default:true)

\*timeout: int (default:10000)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetMotivateCmd",
    "params": {
        "portName": "COM4",
        "q1": 1.0,
        "q2": 2.0,
        "dq1": 1.0,
        "dq2": 2.0,
        "ddq1": 1.0,
        "ddq2": 2.0,
        "isQueued": true,
        "isWaitForFinish": true
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
