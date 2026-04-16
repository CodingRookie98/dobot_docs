### 4.14.4 SetCircleCmd

[**整圆运动**]{style="FONT-SIZE: 14px; FONT-FAMILY: "Microsoft YaHei", "Segoe UI", system-ui, Roboto, "Droid Sans", "Helvetica Neue", sans-serif, Tahoma, "Segoe UI SymbolMyanmar Text", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"}

请求参数 params

  ------------------ --------- ------------ --------------
  字段              类型   是否必填   说明
  portName         string   是          通信端口
  cirPoint          object   是          圆弧上任一点坐标
  toPoint           object   是          圆弧结束点坐标
  isQueued          bool     否         队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  isWaitForFinish   bool     否          等待完成(default:true)
  timeout           int      否          运行超时（60000）
  ------------------ --------- ------------ --------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- ----------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true：操作成功，false：操作失败）
  --------- ------- ----------- ----------------------------------------------

</div>

**KeyWords:**

portName: string

cirPoint: object (float)

toPoint: object (float)

count: int

*isQueued: bool (default:false)

*isWaitForFinish: bool (default:true)

*timeout: int (default:60000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCircleCmd",
    "params": {
        "portName": "COM4",
        "cirPoint": {
            "x": 10,
            "y": 10,
            "z": 10,
            "r": 10
        },
        "toPoint": {
            "x": 210,
            "y": 120,
            "z": 10,
            "r": 0
        },
        "count": 10,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```

OUTPUT：

```json
{

 "id": 1,
  "jsonrpc": "2.0",
 "result": true
}
```
