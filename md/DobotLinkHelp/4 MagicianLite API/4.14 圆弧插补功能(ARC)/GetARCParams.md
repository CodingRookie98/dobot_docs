### 4.14.2 GetARCParams

[**获取圆弧插补功能参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ------------- -----------
  字段       类型   是否必填   说明
  portName   string   是           通信端口
  ----------- --------- ------------- -----------

<div>

响应参数 result

</div>

  ------------------ ---------- ------------ ------------------------------
   字段             类型   是否必填   说明
  xyzVelocity       float     是          圆弧运动 xyz 三坐标轴速度
  rVelocity         float     是          圆弧运动末端旋转速度
  xyzAcceleration   float     是          圆弧运动 xyz 三坐标轴加速度
  rAcceleration     float     是          圆弧运动末端旋转加速度
  ------------------ ---------- ------------ ------------------------------

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
    "method": "dobotlink.MagicianLite.GetARCParams",
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
        "rVelocity": 200,
        "xyzAcceleration": 200,
        "rAcceleration": 200
    }
}
```
