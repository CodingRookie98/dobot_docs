::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](StopAll.html "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetProcessStatus.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> [10 DebuggerLite API](Main.html) \>
:::

::: {#winchm_template_title}
10.7 Input
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: 输入文本到脚本进程**

**KeyWords:**

dpid: int，脚本进程内部ID，控制脚本进程唯一标识

cmd: string, 要传给脚本进程的经过base64转码的文本

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.Input",
    "params": {
        "dpid": 1,
        "cmd"： "xxx"
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
