### 4.2.2 GetDeviceSN

**获取设备序列号**

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

  ----------- -------- ----------- ---------------
  字段       类型    是否必填   说明
  deviceSN   string   是         设备的序列号
  ----------- -------- ----------- ---------------

</div>

<div>

</div>

**KeyWords:**

portName: string

deviceSN: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetDeviceSN",
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
 "deviceSN": "Dobot 2.0"
 }
}
```
