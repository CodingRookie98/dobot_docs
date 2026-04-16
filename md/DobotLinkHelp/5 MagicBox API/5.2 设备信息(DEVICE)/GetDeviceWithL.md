### 5.2.6 GetDeviceWithL

<div>

[**获取设备滑轨状态**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ----------- --------- ----------- ----------------
  字段       类型     是否必填   说明
  portName   string   是          设备的通信端口
  ----------- --------- ----------- ----------------

<div>

响应参数 result

</div>

<div>

</div>

<div>

</div>

<div>

  ----------- ------- ----------- ---------------------------------------
  字段       类型   是否必填   说明
  isEnabled   bool    是         是否使能（True:使能；False：未使能）
  ----------- ------- ----------- ---------------------------------------

</div>

**KeyWords:**

portName: string

isEnabled: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetDeviceWithL",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "isEnabled": true
 }
}
```
