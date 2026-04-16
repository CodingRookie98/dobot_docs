::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetIOMultiplexing.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetIODO.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 5 MagicBox API \> 5.7 端口输入输出功能(EIO) \>
:::

::: {#winchm_template_title}
5.7.2 GetIOMultiplexing
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**获取IO复用**

 

请求参数 params

 

  ----------- --------- ------------ -------------------
   字段        类型      是否必填     说明
   portName    string    是           通信端口
   port        int       是           EIO地址（0\~25）
  ----------- --------- ------------ -------------------

 

<div>

响应参数 result

</div>

 

+-----------------+-----------------+-----------------+-----------------+
|  字段           |   类型          |  是否必填       |   说明          |
+-----------------+-----------------+-----------------+-----------------+
|  multiplex      |  int            | 是              |   复用功能：（  |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 0：IOF          |
|                 |                 |                 | unctionDumm：不 |
|                 |                 |                 | 配置功能，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | []{styl         |
|                 |                 |                 | e="FONT-SIZE: 9 |
|                 |                 |                 | pt; FONT-FAMILY |
|                 |                 |                 | : Times New Rom |
|                 |                 |                 | an; COLOR: rgb( |
|                 |                 |                 | 0,0,0); mso-spa |
|                 |                 |                 | cerun: 'yes'"}[ |
|                 |                 |                 | 1：IOFunctionDO |
|                 |                 |                 | ：IO输出，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [2：            |
|                 |                 |                 | IOFunctionPWM： |
|                 |                 |                 | PWM输出，]{sty  |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 3：IOFunctionDI |
|                 |                 |                 | ：IO输入，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 4               |
|                 |                 |                 | ：IOFunctionADC |
|                 |                 |                 | ：AD输入，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 5：I            |
|                 |                 |                 | OFunctionDIPU： |
|                 |                 |                 | 上拉输入，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 6：I            |
|                 |                 |                 | OFunctionDIPD： |
|                 |                 |                 | 下拉输入。]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | ）              |
+-----------------+-----------------+-----------------+-----------------+
|  port           |  int            | 是              |  E              |
|                 |                 |                 | IO地址（0\~25） |
+-----------------+-----------------+-----------------+-----------------+

**KeyWords:**

portName: string

port: int (0\~25)

multiplex: int (0\~6)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOMultiplexing",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```

 

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "multiplex": 1,
        "port": 1
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
