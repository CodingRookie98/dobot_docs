::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetLightPrompt.html "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetOriginPoint.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 9 MagicianGO API \> 9.4 底盘控制(control) \>
:::

::: {#winchm_template_title}
9.4.16 SetBuzzerSound
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: 设置蜂鸣器音效**

**KeyWords:**

portName: string

index: int （音乐索引）0：关闭， 1：鸣叫， 2：定时关闭， 3：滴，
4：滴滴滴， 5：滴\~滴滴， 6：滴滴滴滴滴 12345 (1234567代表音调dou ruai
mi fa so la xi)， 7：鸣笛提示音：1414

tone: int （音调）（index
0-2有效）(取值范围0-84但低数字区域声音模拟的不好，测试建议选用中间部分如50)

beat: float （节拍）（index 2有效，单位秒）

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; OVERFLOW: auto; WORD-WRAP: normal; FONT-SIZE: 13px; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; MARGIN: 0px 0px 0.5em; ORPHANS: 2; WIDOWS: 2; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetBuzzerSound",
    "params": {
        "portName": "COM4",
        "index": 1,
        "tone": 1,
        "beat": 1
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
