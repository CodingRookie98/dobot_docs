::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](Magician.html "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](StopFirmware.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 11 Download API \>
:::

::: {#winchm_template_title}
10.5 MagicianGO
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: MagicianGO的固件升级接口**

**KeyWords:**

device: string

version: string, 为8位数字版本号，后面补0. 如固件文件版本号是V0.0.0.4,
则version为\"00040000\"

fileName: string,
固件文件的路径，如果路径为空，则使用link下的默认固件文件.
固件前缀为CarTemp，后缀为.bin

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.StartFirmware",
    "params": {
        "device": "MagicianGO",
        "COM": "COM14",
        "version": "00040000",
        "fileName": "D:/download/CarTempV0.0.0.4.bin"
    }
}
```

 

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0.5em 0px; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
}
```

 

Notification: 通知消息，数字是进度

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0.5em 0px; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"5\r\n"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"40.1\r\n"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"100\r\n"
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
