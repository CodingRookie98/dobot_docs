### 8.15.4 AuxSetTeachJoint

**Description: 设置扩展轴示教参数**

**KeyWords:**

portName: string

velocity: List<float>

acceleration: List<float>

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxSetTeachJoint",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "velocity": [100.0, 100.0, 100.0, 100.0],
            "acceleration": [100.0, 100.0, 100.0, 100.0]
        }
    }
}
```
