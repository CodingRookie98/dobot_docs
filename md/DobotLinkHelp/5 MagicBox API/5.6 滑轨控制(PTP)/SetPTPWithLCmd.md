### 5.6.1 SetPTPWithLCmd

<div>

[**执行带滑轨点位功能**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ------------------ --------- ----------- ---------------------------------------
  字段              类型    是否必填   说明
  portName          string   是         通信端口
  l                 float    是         [滑轨运动距离（0-1000） ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  isQueued          bool     否         队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  isWaitForFinish   bool     否         是否等待完成（true:是，false:否）
  ------------------ --------- ----------- ---------------------------------------
响应参数 result

<div>

</div>

<div>

  --------- ------- ----------- ----------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true：设置成功，false：设置失败）
  --------- ------- ----------- ----------------------------------------------

</div>

**KeyWords:**

portName: string

l: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetPTPWithLCmd",
    "params": {
        "portName": "COM4",
        "l": 200,
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
