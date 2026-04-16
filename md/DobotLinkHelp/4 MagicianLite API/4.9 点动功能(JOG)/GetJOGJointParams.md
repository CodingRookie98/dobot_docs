### 4.9.2 GetJOGJointParams

[**获取关节点动参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

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

  --------------- --------------- ------------- -----------------
  字段           类型          是否必填   说明
  velocity       array(float)   是           4 轴关节速度
  acceleration   array(float)   是           4 轴关节加速度
  --------------- --------------- ------------- -----------------

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetJOGJointParams",
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
        "velocity": [15, 15, 15, 30],
        "acceleration": [50, 50, 50, 50]
    }
}
```
