::: {#winchm_template_top}
::: {#winchm_template_button}
[![Previous topic](../template2/btn_prev_n.gif){#winchm_template_prev
border="0"}](SetHardwareEnable.htm "Previous topic")[![Next
topic](../template2/btn_next_n.gif){#winchm_template_next
border="0"}](GetVersion.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \> 7 CR API \> [7.25 Other(unknown)](../$$unsavedpage1.htm) \>
:::

::: {#winchm_template_title}
7.25.20 SetRetraceParams
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
 

功能:

     轨迹复现高级设置

::: {#nstext}
INPUT:

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{    
    "id": 1,    
    "jsonrpc": "2.0",    
    "method": "dobotlink.CR.SetRetraceParams",
    "params": {        
        "portName": "192.168.1.6",
        "data":{
           "multi" : 1          //速度倍数
           "const": 1          //const=1:匀速复现,0:非匀速复现
           "loop":1           //复现次数
          }
    }
}
```

OUTPUT：
:::

<div>

 

</div>

``` {.language-json style="BOX-SIZING: border-box; FONT-SIZE: 13px; OVERFLOW: auto; WORD-WRAP: normal; FONT-FAMILY: Consolas, Monaco, \"Andale Mono\", \"Ubuntu Mono\", monospace; BACKGROUND: rgb(245,242,240); WHITE-SPACE: pre; WORD-SPACING: 0px; TEXT-TRANSFORM: none; WORD-BREAK: normal; FONT-WEIGHT: 400; COLOR: black; PADDING-BOTTOM: 1em; FONT-STYLE: normal; TEXT-ALIGN: left; PADDING-TOP: 1em; PADDING-LEFT: 1em; ORPHANS: 2; WIDOWS: 2; MARGIN: 0px 0px 0.5em; LETTER-SPACING: normal; LINE-HEIGHT: 1.5; PADDING-RIGHT: 1em; TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; border-radius: 3px; text-shadow: white 0px 1px; tab-size: 4; hyphens: none"}
{ 
    "id": 1, 
    "jsonrpc": "2.0",
     "result":{"value":true/false} 
}
```

 
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::
