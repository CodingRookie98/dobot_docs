### 5.2.1 SetDeviceSN

**设置设备序列号**

请求参数 params

  ----------- --------- ----------- ---------------------------------------
  字段       类型     是否必填   说明
  portName   string   是          设备的通信端口
  deviceSN   string   是         需要设置的序列号（以 DT14 作为开头）
  ----------- --------- ----------- ---------------------------------------

<div>

响应参数 result

</div>

<div>

</div>

<div>

  ----------- -------- ----------- ------------
  字段       类型    是否必填   说明
  deviceSN   string   是         设备序列号
  ----------- -------- ----------- ------------

</div>

<div>

</div>

**KeyWords:**

portName: string

deviceSN: string (start with 'DT14')

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetDeviceSN",
    "params": {
        "portName": "COM4",
        "deviceSN": "DT1418080700"
    }
}
```

OUTPUT:

```json
{
 "id": 1,

 "jsonrpc": "2.0",
   "result": {
 "deviceSN": "u0002"
   }
}
```
