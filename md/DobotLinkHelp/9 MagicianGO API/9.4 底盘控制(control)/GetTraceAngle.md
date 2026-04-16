### 9.4.24 GetImuAngle

**Description: 获取IMU航向角**

**KeyWords:**

portName: string

yaw: float(IMU航向角)°

roll: float(IMU横滚角)°

pitch: float(IMU俯仰角)°

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetImuAngle",
    "params": {
        "portName": "COM4"
    }
}
```
