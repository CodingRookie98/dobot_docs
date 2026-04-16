::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](PTP-tips.htm "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetRCmd.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 4 MagicianLite API \> [4.10 点到点运动指令(PTP)](PTP-tips.htm)
\>
:::

::: {#winchm_template_title}
4.10.1 SetPTPCmd
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**执行点位功能**

 

<div>

请求参数 params

</div>

 

+-----------------+-----------------+-----------------+-----------------+
|  字段           |  类型           |  是否必填       |  说明           |
+-----------------+-----------------+-----------------+-----------------+
| portName        |  string         |  是             |  通信端口       |
+-----------------+-----------------+-----------------+-----------------+
| ptpMode         |  int            |  是             |  运动模式（     |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 0:门型运动，参  |
|                 |                 |                 | 数为目标点参数  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 1:关节运动，参  |
|                 |                 |                 | 数为目标点参数  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 2:直线运动，参  |
|                 |                 |                 | 数为目标点参数  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 3:门            |
|                 |                 |                 | 型运动，参数为  |
|                 |                 |                 | 目标点关节角度  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 4:关            |
|                 |                 |                 | 节运动，参数为  |
|                 |                 |                 | 目标点关节角度  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 5:直            |
|                 |                 |                 | 线运动，参数为  |
|                 |                 |                 | 目标点关节角度  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 6               |
|                 |                 |                 | :关节运动增量模 |
|                 |                 |                 | 式，参数为目标  |
|                 |                 |                 | 点关节角度增量  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 7:直线运动增    |
|                 |                 |                 | 量模式，参数为  |
|                 |                 |                 | 目标点坐标增量  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 8:关节运动增    |
|                 |                 |                 | 量模式，参数为  |
|                 |                 |                 | 目标点坐标增量  |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 |                 | 9:门型运        |
|                 |                 |                 | 动，平移时运动  |
|                 |                 |                 | 模式为直线运动  |
|                 |                 |                 | ）              |
+-----------------+-----------------+-----------------+-----------------+
|  x              |  float          |  是             |  当前的x位置    |
+-----------------+-----------------+-----------------+-----------------+
|  y              |  float          |  是             |  当前的y位置    |
+-----------------+-----------------+-----------------+-----------------+
|  z              |  float          |  是             |  当前的z位置    |
+-----------------+-----------------+-----------------+-----------------+
|  r              |  float          |  是             |  当前的r位置    |
+-----------------+-----------------+-----------------+-----------------+
| isQueued        |  bool           |  否             |  队列指令（t    |
|                 |                 |                 | rue：指令排队执 |
|                 |                 |                 | 行，false：打断 |
|                 |                 |                 | 当前执行的任务  |
|                 |                 |                 | ，直接插入执行  |
|                 |                 |                 | ）默认：false   |
+-----------------+-----------------+-----------------+-----------------+
| isWaitForFinish |  bool           |  否             |  是否等         |
|                 |                 |                 | 待指令完成（[t  |
|                 |                 |                 | rue：等待指令完 |
|                 |                 |                 | 成才返回，fals  |
|                 |                 |                 | e：收到指令立即 |
|                 |                 |                 | 返回]{style="F  |
|                 |                 |                 | ONT-SIZE: 14px; |
|                 |                 |                 |  FONT-FAMILY: \ |
|                 |                 |                 | "Microsoft YaHe |
|                 |                 |                 | i\", \"Segoe UI |
|                 |                 |                 | \", system-ui,  |
|                 |                 |                 | Roboto, \"Droid |
|                 |                 |                 |  Sans\", \"Helv |
|                 |                 |                 | etica Neue\", s |
|                 |                 |                 | ans-serif, Taho |
|                 |                 |                 | ma, \"Segoe UI  |
|                 |                 |                 | SymbolMyanmar T |
|                 |                 |                 | ext\", 微软雅黑 |
|                 |                 |                 | ; WHITE-SPACE:  |
|                 |                 |                 |  pre-wrap; WORD |
|                 |                 |                 | -SPACING: 0px;  |
|                 |                 |                 | TEXT-TRANSFORM: |
|                 |                 |                 |  none; FLOAT: n |
|                 |                 |                 | one; FONT-WEIGH |
|                 |                 |                 | T: 400; COLOR:  |
|                 |                 |                 | rgb(23,26,29);  |
|                 |                 |                 | FONT-STYLE: nor |
|                 |                 |                 | mal; TEXT-ALIGN |
|                 |                 |                 | : left; ORPHANS |
|                 |                 |                 | : 2; WIDOWS: 2; |
|                 |                 |                 |  DISPLAY: inlin |
|                 |                 |                 | e !important; L |
|                 |                 |                 | ETTER-SPACING:  |
|                 |                 |                 | normal; BACKGRO |
|                 |                 |                 | UND-COLOR: rgb( |
|                 |                 |                 | 255,255,255); T |
|                 |                 |                 | EXT-INDENT: 0px |
|                 |                 |                 | ; font-variant- |
|                 |                 |                 | ligatures: norm |
|                 |                 |                 | al; font-varian |
|                 |                 |                 | t-caps: normal; |
|                 |                 |                 |  -webkit-text-s |
|                 |                 |                 | troke-width: 0p |
|                 |                 |                 | x; text-decorat |
|                 |                 |                 | ion-style: init |
|                 |                 |                 | ial; text-decor |
|                 |                 |                 | ation-color: in |
|                 |                 |                 | itial; text-dec |
|                 |                 |                 | oration-thickne |
|                 |                 |                 | ss: initial"}） |
+-----------------+-----------------+-----------------+-----------------+
| timeout         |  bool           |  否             | 运动            |
|                 |                 |                 | 超时，默认为5s  |
+-----------------+-----------------+-----------------+-----------------+

 

 

 

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

ptpMode: int (0\~9)

x: float

y: float

z: float

r: float

\*isQueued: bool (default:true)

\*isWaitForFinish: bool (default:true)

\*timeout: int (default:5000)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetPTPCmd",
    "params": {
        "portName": "COM4",
        "ptpMode": 1,
        "x": 210,
        "y": 100,
        "z": 10,
        "r": 0,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```

 

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
    {
  "id": 1,
  "jsonrpc": "2.0", 
  "result": true
}
```
:::

<div>

 

</div>
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
