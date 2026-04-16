### 5.4.2 GetServoAngle

[**获取舵机的角度**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

<div>

</div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

  -------- ------- ----------- ----------------------
  字段    类型   是否必填   说明
  angle   int    是         舵机的角度 (+/-180)
  index   int    是         舵机序号
  -------- ------- ----------- ----------------------

</div>

<div>

</div>

**KeyWords:**

portName: string

index: int

angle: float (+/-180)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetServoAngle",
    "params": {
        "portName": "COM4",
        "index": 2
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "angle": -270,
 "index": 2
 }

}
```
