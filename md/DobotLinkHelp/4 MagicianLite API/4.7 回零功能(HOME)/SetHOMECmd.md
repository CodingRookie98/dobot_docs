### 4.7.3 SetHOMECmd

<div>

[**执行回零命令**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

  ------------------- --------- ------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  字段              类型   是否必填   说明
  portName          string   是         通信端口
  isQueued          bool     否         队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行）
   isWaitForFinish   bool     否         是否等待指令完成（ [true：等待指令完成才返回，false：收到指令立即返回]{style="FONT-SIZE: 14px; FONT-FAMILY: "Microsoft YaHei", "Segoe UI", system-ui, Roboto, "Droid Sans", "Helvetica Neue", sans-serif, Tahoma, "Segoe UI SymbolMyanmar Text", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"}）
  timeout            int      否          运动超时，默认为8秒
  ------------------- --------- ------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
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

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:8000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetHOMECmd",
    "params": {
        "portName": "COM4",
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true

}
```
