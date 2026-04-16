### 5.1.2 ConnectDobot

**连接当前设备**

<div>

</div>

<div>

请求参数 params

</div>

<div>

</div>

<div>

  ----------- --------- ----------- ----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- ----------

</div>

<div>

</div>

<div>

</div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

  ------------------ --------- ------------ -----------
  字段              类型    是否必填   说明
  firmwareName      string   是          固件名称
  firmwareVersion   string   是          固件版本
  productName       string   是          设备名称
  ------------------ --------- ------------ -----------

</div>

<div>

</div>

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.ConnectDobot",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
 {
 "id": 14,
 "jsonrpc": "2.0",
 "result": {
 "firmwareName": "Dobot",
 "firmwareVersion": "",
 "productName": ""
 }
}
```
