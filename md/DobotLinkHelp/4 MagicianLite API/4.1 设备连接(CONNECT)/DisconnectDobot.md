::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](ConnectDobot.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../device/SetDeviceSN.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> 4.1 设备连接(CONNECT) \>
:::

::: {#winchm_template_title}
4.1.3 DisconnectDobot
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**断开设备连接**

 

<div>

请求参数 params

</div>

<div>

 

</div>

<div>

 

</div>

<div>

  ------------- ---------- ------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   字段          类型       是否必填     说明 
   portName      string     是          通信端口
   queueStop     bool       是          [停止队列，默认为true(true：开启[停止队列]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}操作，false：关闭停止队列操作)]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}
   queueClear    bool       是          [清除队列，默认为true(true：开启清除[队列]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}操作，false：关闭清除队列操作)]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}
  ------------- ---------- ------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

</div>

<div>

 

</div>

<div>

响应参数 result

</div>

<div>

 

</div>

<div>

  --------- ------- ----------- ----------------------------------------------------
   字段     类型    是否必填    说明 
   result   bool    是           设备的连接状态（true：连接成功，false：连接失败）
  --------- ------- ----------- ----------------------------------------------------

</div>

<div>

 

</div>

 

**KeyWords:**

portName: string

\*queueStop: bool (default:true)

\*queueClear: bool (default:true)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.DisconnectDobot",
    "params": {
        "portName": "COM4",
        "queueStop": true,
        "queueClear": true
    }
}
```

 

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
     
{
    "id": 56,
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
