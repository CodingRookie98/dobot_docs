::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](AuxSetStructure.htm "Previous topic")[![Next
topic](../../template2/btn_next_n.gif){#winchm_template_next
border="0"}](../../MagicianGO/connect/ConnectDobot.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 8 MagicianPro API \> 8.15 扩展轴(AUX) \>
:::

::: {#winchm_template_title}
8.15.9 AuxGetStructure
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
::: {#nstext}
**Description: 获取扩展轴其他参数**

**KeyWords:**

portName: string

 

INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxGetStructure",
    "params": {
        "portName": "192.168.1.6"
    }
}
```

OUTPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "auxJoint":3, //扩展轴数量
        "type":[0,0,0], //0-关节，1-直线
        "limits":
        [
            [0, 0],--范围限制
            [0, 0],
            [0, 0]
        ],
        "motors": [
            {
                "composite": false,
                "encoder": {
                    "bitNum": 17,--编码器位数
                    "type": ""
                },
                "gearBox": {
                    "den": 50, --减速比分母
                    "num": 1 --减速比分子
                },
                "motor": {
                    "inverted": false, --电机转动方向
                    "limit": 5500, --最大转速
                    "rated": 5000, --额定转速
                    "type": ""
                },
                "positionScaling": {
                    "den": 1,
                    "num": 360
                },
                "simulated": true --虚/实轴
            },
            {
                "composite": false,
                "encoder": {
                    "bitNum": 17,
                    "type": ""
                },
                "gearBox": {
                    "den": 50,
                    "num": 1
                },
                "motor": {
                    "inverted": false,
                    "limit": 5500,
                    "rated": 5000,
                    "type": ""
                },
                "positionScaling": {
                    "den": 1,
                    "num": 360
                },
                "simulated": true
            },
            {
                "composite": false,
                "encoder": {
                    "bitNum": 17,
                    "type": ""
                },
                "gearBox": {
                    "den": 50,
                    "num": 1
                },
                "motor": {
                    "inverted": false,
                    "limit": 5500,
                    "rated": 5000,
                    "type": ""
                },
                "positionScaling": {
                    "den": 1,
                    "num": 360
                },
                "simulated": true
            }
        ]
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
