### 3.5.2 ResetPose

**KeyWords:**

portName: string

manualEnable: bool

*rearArmAngle: float (manualEnable = true)

*frontArmAngle: float (manualEnable = true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.ResetPose",
    "params": {
        "portName": "COM4",
        "manualEnable": true,
        "rearArmAngle": 100,
        "frontArmAngle": 150
    }
}
```
