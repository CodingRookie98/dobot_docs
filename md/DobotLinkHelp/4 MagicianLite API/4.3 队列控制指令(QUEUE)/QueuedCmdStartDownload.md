### 4.3.4 QueuedCmdStartDownload

<div>

[**启动指令队列下载**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

<div>

</div>

  -------------- --------- ------------ ---------------------------------------------------
  字段          类型    是否必填   说明
  portName      string   是          设备的通信端口
  totalLoop     int      是          [总循环次数]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri"}
  linePerLoop   int      是          [每条语句的循环次数]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri"}[]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri"}
  -------------- --------- ------------ ---------------------------------------------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- ---------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true：操作成功，false：操作失败）
  --------- ------- ----------- ---------------------------------------------

</div>

<div>

</div>

**KeyWords:**

portName: string

totalLoop: int

linePerLoop: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.QueuedCmdStartDownload",
    "params": {
        "portName": "COM4",
        "totalLoop": 1,
        "linePerLoop": 1
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
