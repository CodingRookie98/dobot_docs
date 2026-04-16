### 4.15.1 SetWAITCmd

[**执行时间等待功能**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ----------- -----------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  delay      int      是         等待时间（单位：ms）
  ----------- --------- ----------- -----------------------

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

delay: int

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetWAITCmd",
    "params": {
        "portName": "COM4",
        "delay": 500
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
