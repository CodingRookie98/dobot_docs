### 4.9.4 GetJOGCoordinateParams

[**获取坐标轴点动参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

<div>

请求参数 params

</div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

  ----------- --------- ------------ -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ------------ -----------

<div>

响应参数 result

</div>

  --------------- --------------- ------------ ---------------------------------------------------------------
  字段           类型          是否必填   说明
  velocity       array(float)   是          [ 4 轴坐标轴（x,y,z,r）速度 (取值范围：0-225) ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  acceleration   array(float)   是          [4 轴坐标轴（x,y,z,r）加速度 (取值范围：0-100) ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  --------------- --------------- ------------ ---------------------------------------------------------------
**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetJOGCoordinateParams",
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
        "velocity": [60, 60, 60, 60],
        "acceleration": [60, 60, 60, 60]
    }
}
```
