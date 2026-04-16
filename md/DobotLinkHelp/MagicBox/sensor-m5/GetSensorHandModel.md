::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetSensorHandModel.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../sensor-hand/5.13.1_IsSensorHandModel.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> [12 AI传感器套件](../../$$unsavedpage2.htm) \> 12.1
m5传感器(SENSOR-M5) \>
:::

::: {#winchm_template_title}
12.1.33 GetSensorHandModel
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**获取手势识别模块**

 

请求参数 params

 

  ----------- --------- ----------- -----------------
   字段       类型       是否必填   说明 
   portName    string    是          通信端口
   port        int       是          端口号（0\~5）
  ----------- --------- ----------- -----------------

 

响应参数 result

 

+-----------------+-----------------+-----------------+-----------------+
|  字段           | 类型            |  是否必填       | 说明            |
+-----------------+-----------------+-----------------+-----------------+
|  data           |  string         |  是             | 识别值：        |
|                 |                 |                 |                 |
|                 |                 |                 | 返回            |
|                 |                 |                 | 值的每个位数代  |
|                 |                 |                 | 表一个手势位置  |
|                 |                 |                 |                 |
|                 |                 |                 | ( // REGISTER 0 |
|                 |                 |                 |                 |
|                 |                 |                 | GES_RIGHT_FLAG  |
|                 |                 |                 | = BIT(0),       |
|                 |                 |                 |                 |
|                 |                 |                 | GES_LEFT_FLAG = |
|                 |                 |                 | BIT(1),         |
|                 |                 |                 |                 |
|                 |                 |                 | GES_UP_FLAG =   |
|                 |                 |                 | BIT(2),         |
|                 |                 |                 |                 |
|                 |                 |                 | GES_DOWN_FLAG = |
|                 |                 |                 | BIT(3),         |
|                 |                 |                 |                 |
|                 |                 |                 | G               |
|                 |                 |                 | ES_FORWARD_FLAG |
|                 |                 |                 | = BIT(4),       |
|                 |                 |                 |                 |
|                 |                 |                 | GE              |
|                 |                 |                 | S_BACKWARD_FLAG |
|                 |                 |                 | = BIT(5),       |
|                 |                 |                 |                 |
|                 |                 |                 | GES             |
|                 |                 |                 | _CLOCKWISE_FLAG |
|                 |                 |                 | = BIT(6),       |
|                 |                 |                 |                 |
|                 |                 |                 | GES_COUNT       |
|                 |                 |                 | _CLOCKWISE_FLAG |
|                 |                 |                 | = BIT(7),       |
|                 |                 |                 |                 |
|                 |                 |                 | // REGISTER 1   |
|                 |                 |                 |                 |
|                 |                 |                 | GES_WAVE_FLAG = |
|                 |                 |                 | BIT(0),         |
|                 |                 |                 | READ_ERR =      |
|                 |                 |                 | 0xff）          |
+-----------------+-----------------+-----------------+-----------------+

 

 

 

**KeyWords:**

portName: string

port: int, 端口，0\~5

data: int

// REGISTER 0

GES_RIGHT_FLAG = BIT(0), GES_LEFT_FLAG = BIT(1), GES_UP_FLAG = BIT(2),
GES_DOWN_FLAG = BIT(3), GES_FORWARD_FLAG = BIT(4), GES_BACKWARD_FLAG =
BIT(5), GES_CLOCKWISE_FLAG = BIT(6), GES_COUNT_CLOCKWISE_FLAG = BIT(7),

// REGISTER 1

GES_WAVE_FLAG = BIT(0), READ_ERR = 0xff,

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetSensorHandModel",
    "params": {
        "portName": "COM4",
        "port": 2 
    }
}
```

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "data": 255
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
