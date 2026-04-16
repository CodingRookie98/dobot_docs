::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetWorldCoordinateMovePoint.htm "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetTraceCenterARC.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 9 MagicianGO API \> 9.4 底盘控制(control) \>
:::

::: {#winchm_template_title}
9.4.10 SetArcRad
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: 设置半径圆弧轨迹功能，根据转动半径，角度做圆弧运动**

**KeyWords:**

portName: string

velocity: float（走圆弧轨迹的速度，单位
°/s（度/秒），正值表示逆时针旋转，负值表示顺时针旋转 ）

radius: float（圆弧轨迹半径）(cm)

angle: float（小车绕圆弧转动角度）(deg/s)

mode: int(选择绕圆弧轨迹行走的模式，取值\[1, 2\]，
1-切向运动，2-刷锅运动)

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetArcRad",
    "params": {
        "portName": "COM4",
        "velocity": 10.0,
        "radius": 10.0,
        "angle": 10.0,
        "mode": 1
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
