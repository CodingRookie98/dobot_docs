### 4.10.4 GetPTPJointParams

**获取关节点位参数**

<div>

</div>

<div>

请求参数 params

</div>

  ----------- --------- ------------ -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ------------ -----------

响应参数 result

  --------------- --------------- ------------ ----------------------------
  字段           类型          是否必填   说明
  velocity       array(float)   是          PTP 模式下 4 轴关节速度
  acceleration   array(float)   是          PTP 模式下 4 轴关节加速度
  --------------- --------------- ------------ ----------------------------

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPTPJointParams",
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
        "velocity": [200, 200, 200, 200],
        "acceleration": [200, 200, 200, 200]
    }
}
```
