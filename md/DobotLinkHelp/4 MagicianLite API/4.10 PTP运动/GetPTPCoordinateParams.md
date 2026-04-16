### 4.10.6 GetPTPCoordinateParams

<div>

[**设置坐标轴点位参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

  ----------- --------- ------------ -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ------------ -----------

响应参数 result

  ------------------ -------- ------------ ----------------------------------
  字段             类型    是否必填   说明
  xyzVelocity       float   是          PTP 模式下 xyz 3 轴坐标轴速度
  rVelocity         float   是          PTP 模式下末端速度
  xyzAcceleration   float   是          PTP 模式下 xyz 3 轴坐标轴加速度
  rAcceleration     float   是          PTP 模式下末端加速度
  ------------------ -------- ------------ ----------------------------------

**KeyWords:**

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPTPCoordinateParams",
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
        "xyzVelocity": 200,
        "rVelocity": 100,
        "xyzAcceleration": 200,
        "rAcceleration": 100
    }
}
```
