::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](GetPackPoint.htm "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetJumpStructure.htm "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 7 CR API \> [7.25 Other(unknown)](../$$unsavedpage1.htm) \>
:::

::: {#winchm_template_title}
7.25.9 SetJumpStructure
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
功能:

设置jump速度参数\
\
\
\

::: {#nstext}
INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
 "id":1,
 "jsonrpc":"2.0",
 "method":"dobotlink.CR.SetJumpStructure",
 "params":{
  "portName":"192.168.5.1",
  "data":{"motors":[{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":false,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true}],"structure":{"L1":147,"L2":0,"L3":0,"L4":143.028,"L5":119.9334,"L6":104.5,"L7":0,"a1":0,"a2":-427.3999,"a3":-356.1736,"a4":0,"a5":0,"a6":0,"armSingularity12":100,"elbowSingularity12":10,"inclinationAngle":0.66,"limits":[[-178,178],[-178,178],[-160,160],[-178,178],[-178,178],[-357,357]],"rotationAngle":0.55,"wristSingularity12":10}}
 }
}
```
:::

OUTPUT：

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
}
```
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::
