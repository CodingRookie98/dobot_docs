### 4.3.2 QueuedCmdStop

[**停止指令队列**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ------------ --------- ----------- -------------------------------------------
  字段        类型     是否必填   说明
  portName    string   是          设备的通信端口
  forceStop   bool      是         [强制停止队列（true:开启强制停止队列，false:关闭强制停止队列）]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri"}
  ------------ --------- ----------- -------------------------------------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- ---------------------------------------------
  字段     类型   是否必填   说明
  result   bool    否          响应结果（true：操作成功，false：操作失败）
  --------- ------- ----------- ---------------------------------------------

</div>

**KeyWords:**

portName: string

*forceStop: bool (default: false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.QueuedCmdStop",
    "params": {
        "portName": "COM4",
        "forceStop": false
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
