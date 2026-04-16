### 5.2.5 SetDeviceWithL

<div>

[**设置设备滑轨状态**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ---------- ------- ----------- ------------------------------------
  字段      类型   是否必填   说明
  enable    bool    是          使能滑轨。True:使能；False：未使能
  version   int    是         滑轨版本号（0：V1版本，1：V2版本）
  ---------- ------- ----------- ------------------------------------

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

enable: bool

version: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetDeviceWithL",
    "params": {
        "portName": "COM4",
        "enable": true,
        "version": 1
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
