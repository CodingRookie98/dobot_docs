### 4.2.3 SetDeviceName

**设置设备名称**

请求参数 params

  ------------- --------- ----------- ---------------------
  字段         类型     是否必填   说明
  portName     string   是          设备的通信端口
  deviceName   string   是         需要设置的设备名称
  ------------- --------- ----------- ---------------------

<div>

响应参数 result

</div>

<div>

</div>

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

deviceName: string

INPUT

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "method": "dobotlink.MagicianLite.SetDeviceName",
 "params": {
 "portName": "COM15",
 "deviceName": "Dobot123"
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
