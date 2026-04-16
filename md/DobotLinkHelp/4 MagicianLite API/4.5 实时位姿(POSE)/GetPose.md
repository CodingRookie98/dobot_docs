### 4.5.1 GetPose

[**获取实时位置**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

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

  ------------- --------------- ------------ -------------------------------------------
  字段         类型          是否必填   说明
  x            float          是          当前x的位置
  y            float          是          当前y的位置
  z            float          是          当前z的位置
  r            float          是          当前r的位置
  jointAngle   array(float)   是          机械臂 4轴（底座、大臂、小臂、末端）角度
  ------------- --------------- ------------ -------------------------------------------

</div>

[]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

**KeyWords:**

portName: string

x: float

y: float

z: float

r: float

jointAngle: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPose",
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
        "x": 134.01580810546875,
        "y": -5.637601852416992,
        "z": 34.831390380859375,
        "r": -2.4088234901428223,
        "jointAngle": [-2.4088234901428223, 10.456664085388184, 41.771934509277344, 0]
    }
}
```
