::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetSpeedDefault.htm "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](SetApiUpdate.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 7 CR API \> [7.25 Other(unknown)](../$$unsavedpage1.htm) \>
:::

::: {#winchm_template_title}
7.25.12 GetSpeedDefault
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
功能:

功能: 获取所有速度参数默认值

::: {#nstext}
INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetSpeedDefault",
    "params": {
        "portName": "192.168.5.1"
    }
}
```
:::

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{

    "id": 1,

    "jsonrpc": "2.0",

     "result":{"common":{"ratio":{"def":50,"max":100,"min":1}},"dragSensivity":{"j1":{"def":50,"max":90,"min":1},"j2":{"def":50,"max":90,"min":1},"j3":{"def":50,"max":90,"min":1},"j4":{"def":50,"max":90,"min":1},"j5":{"def":50,"max":90,"min":1},"j6":{"def":50,"max":90,"min":1}},"playback":{"arch":{"endHeight":{"def":20,"max":1300,"min":1},"startHeight":{"def":20,"max":1300,"min":1},"zLimit":{"def":50,"max":1300,"min":1}},"coordinate":{"acceleration":[{"def":10000,"max":999999,"min":1},{"def":10000,"max":999999,"min":1},{"def":10000,"max":999999,"min":1},{"def":900,"max":999999,"min":1},{"def":900,"max":999999,"min":1},{"def":900,"max":999999,"min":1}],"jerk":[{"def":18000,"max":999999,"min":1},{"def":18000,"max":999999,"min":1},{"def":18000,"max":999999,"min":1},{"def":9000,"max":999999,"min":1},{"def":9000,"max":999999,"min":1},{"def":9000,"max":999999,"min":1}],"velocity":[{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1}]},"joint":{"acceleration":[{"def":200,"max":999999,"min":1},{"def":200,"max":999999,"min":1},{"def":200,"max":999999,"min":1},{"def":500,"max":999999,"min":1},{"def":500,"max":999999,"min":1},{"def":500,"max":999999,"min":1}],"jerk":[{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":5000,"max":999999,"min":1},{"def":5000,"max":999999,"min":1},{"def":5000,"max":999999,"min":1}],"velocity":[{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1}]}},"teach":{"coordinate":{"acceleration":[{"def":300,"max":999999,"min":1},{"def":300,"max":999999,"min":1},{"def":300,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1}],"velocity":[{"def":50,"max":999999,"min":1},{"def":50,"max":999999,"min":1},{"def":50,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1}]},"joint":{"acceleration":[{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1}],"velocity":[{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1}]}}}

}
```
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::
