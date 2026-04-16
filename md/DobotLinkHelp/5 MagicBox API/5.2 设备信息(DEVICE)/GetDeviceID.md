### 5.2.7 GetDeviceID

**获取设备ID**

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

  ----------- ------------ ----------- ---------------
  字段       类型        是否必填   说明
  deviceID   array(int)   是         设备的ID数据
  ----------- ------------ ----------- ---------------

</div>

**KeyWords:**

portName: string

deviceID: array(int)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetDeviceID",
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
 "deviceID": [48, 255, 218]

 }
}
```
