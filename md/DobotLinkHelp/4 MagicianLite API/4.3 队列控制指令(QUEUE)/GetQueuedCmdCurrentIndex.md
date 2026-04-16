### 4.3.6 GetQueuedCmdCurrentIndex

<div>

[**获取指令队列索引**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

<div>

响应参数 result

</div>

<div>

</div>

<div>

</div>

<div>

+-----------------+-----------------+-----------------+-----------------+
| 字段           | 类型           | 是否必填       | 说明           |
+-----------------+-----------------+-----------------+-----------------+
| queuedCmdIndex | int             | 是             | {s          |
|                 |                 |                 | tyle="FONT-SIZE |
|                 |                 |                 | : medium; WHITE |
|                 |                 |                 | -SPACE: normal; |
|                 |                 |                 |  WORD-SPACING:  |
|                 |                 |                 | 0px; TEXT-TRANS |
|                 |                 |                 | FORM: none; FON |
|                 |                 |                 | T-WEIGHT: 400;  |
|                 |                 |                 | COLOR: rgb(0,0, |
|                 |                 |                 | 0); FONT-STYLE: |
|                 |                 |                 |  normal; ORPHAN |
|                 |                 |                 | S: 2; WIDOWS: 2 |
|                 |                 |                 | ; LETTER-SPACIN |
|                 |                 |                 | G: normal; TEXT |
|                 |                 |                 | -INDENT: 0px; f |
|                 |                 |                 | ont-variant-lig |
|                 |                 |                 | atures: normal; |
|                 |                 |                 |  font-variant-c |
|                 |                 |                 | aps: normal; -w |
|                 |                 |                 | ebkit-text-stro |
|                 |                 |                 | ke-width: 0px;  |
|                 |                 |                 | text-decoration |
|                 |                 |                 | -style: initial |
|                 |                 |                 | ; text-decorati |
|                 |                 |                 | on-color: initi |
|                 |                 |                 | al; text-decora |
|                 |                 |                 | tion-thickness: |
|                 |                 |                 |  initial" ksdoc |
|                 |                 |                 | clipboard="ksDo |
|                 |                 |                 | cClipboardId:'{ |
|                 |                 |                 | 10364193-f0ce-b |
|                 |                 |                 | b57-d0df-1e7bec |
|                 |                 |                 | 861d33-47399316 |
|                 |                 |                 | 516}';from:'wps |
|                 |                 |                 | ';priorityForma |
|                 |                 |                 | t:'Kingsoft WPS |
|                 |                 |                 |  9.0 Format';mi |
|                 |                 |                 | metypes:'Kingso |
|                 |                 |                 | ft WPS 9.0 Form |
|                 |                 |                 | at;text/html'"} |
|                 |                 |                 | [[]{style="F    |
|                 |                 |                 | ONT-SIZE: 10.5p |
|                 |                 |                 | t; FONT-FAMILY: |
|                 |                 |                 |  Calibri"}]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 10.5pt; FONT-FA |
|                 |                 |                 | MILY: Calibri"} |
|                 |                 |                 |                 |
|                 |                 |                 | [队列命令       |
|                 |                 |                 | 索引]{style="FO |
|                 |                 |                 | NT-SIZE: 10.5pt |
|                 |                 |                 | ; FONT-FAMILY:  |
|                 |                 |                 | Calibri"}[]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 10.5pt; FONT-FA |
|                 |                 |                 | MILY: Calibri"} |
|                 |                 |                 | |
+-----------------+-----------------+-----------------+-----------------+

</div>

**KeyWords:**

portName: string

queuedCmdIndex: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetQueuedCmdCurrentIndex",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "queuedCmdIndex": 56
 }
}
```
