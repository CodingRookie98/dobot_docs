::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](Main.html "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](Start.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> [10 DebuggerLite API](Main.html) \>
:::

::: {#winchm_template_title}
10.1 Prepare
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: 初始化脚本进程**

**KeyWords:**

script: string，base64转码后的代码

\*portName: string，可选，使用EDU模块的时候用到

\*host: string，可选，使用EDU模块的时候用到

\*token: string，可选，使用EDU模块的时候用到

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.Prepare",
    "params": {
        "script": "aW1wb3J0IHRpbWUKCndoaWxlIDE6CiAgICBwcmludCgxMTExKQogICAgdGltZS5zbGVlcCgxKQ",
        "portName": "COM4",
        "host": "http://dev.dobotlab.com",
        "token": "CiAgICBwcmludCgogICAgdGltZ"
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
