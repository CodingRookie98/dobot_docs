### 4.10.10 GetPTPCommonParams

<div>

[**获取点位公共参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

  ----------- --------- ------------ -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ------------ -----------

响应参数 result

  -------------------- -------- ------------ --------------------------------------------
  字段               类型    是否必填   说明
  velocityRatio       float   是          PTP 模式速度比例，关节和坐标轴模式共用
  accelerationRatio   float   是          PTP 模式加速度比例，关节和坐标轴模式共用
  -------------------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

velocityRatio: float

accelerationRatio: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPTPCommonParams",
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
 "accelerationRatio": 123,
 "velocityRatio": 123
 }
}
```
