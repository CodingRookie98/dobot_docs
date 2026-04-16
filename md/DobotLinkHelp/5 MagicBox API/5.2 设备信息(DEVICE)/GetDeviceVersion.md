### 5.2.4 GetDeviceVersion

**获取设备版本号**

请求参数 params

  ------------- --------- ----------- ----------------
  字段         类型     是否必填   说明
  portName     string   是          设备的通信端口
  deviceName   string   是         设备名称
  ------------- --------- ----------- ----------------

<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------------- -------- ------------ -------------
  字段           类型   是否必填   说明
  majorVersion   int     是          主要版本号
  minorVersion   int     是          次要版本号
  revision       int     是          修订版本号
  hwVersion      int     是          设备版本号
  --------------- -------- ------------ -------------

</div>

**KeyWords:**

portName: string

majorVersion: int

minorVersion: int

revision: int

hwVersion: int

deviceName: 设备名称

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetDeviceVersion",
    "params": {
        "portName": "COM4",
        "deviceName":"MagicBox"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "majorVersion": 2,
        "minorVersion": 0,
        "revision": 0,
        "hwVersion": 6
    }
}
```
