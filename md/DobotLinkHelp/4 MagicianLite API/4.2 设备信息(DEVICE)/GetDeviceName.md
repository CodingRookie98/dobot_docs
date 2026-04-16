### 4.2.4 GetDeviceName

**获取设备名称**

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

  ------------- -------- ----------- -----------
  字段         类型    是否必填   说明
  deviceName   string   是         设备名称
  ------------- -------- ----------- -----------

</div>

**KeyWords:**

portName: string

deviceName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetDeviceName",
    "params": {
        "portName": "COM15"
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "deviceName": "Dobot123"
 }
}
```
