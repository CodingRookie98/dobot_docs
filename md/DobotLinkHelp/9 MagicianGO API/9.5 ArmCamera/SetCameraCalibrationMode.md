### 9.5.5 SetArmCameraCalibrationMode

**Description: 设置K210校准模式状态**

**KeyWords:**

portName: string

isEnableCali: int, 校准模式设置，0关闭校准；1开启校准

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetArmCameraCalibrationMode",
    "params": {
        "portName": "COM4",
        "isEnableCali": 0/1
    }
}
```
