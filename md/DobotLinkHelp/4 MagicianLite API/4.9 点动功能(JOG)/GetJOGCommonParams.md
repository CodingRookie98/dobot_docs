### 4.9.6 GetJOGCommonParams

[**获取点动公共参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

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

  -------------------- -------- ------------ -------------------------------------------------------
  字段                类型   是否必填   说明
  accelerationRatio   float    是          [ 速度比例，关节点动和坐标轴点动共用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  velocityRatio       float    是           [ 加速度比例，关节点动和坐标轴点动共用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  -------------------- -------- ------------ -------------------------------------------------------
**KeyWords:**

portName: string

velocityRatio: float

accelerationRatio: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetJOGCommonParams",
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
 "accelerationRatio": 50,
 "velocityRatio": 100
 }
}
```
