### 6.12.3 SetInchParam

**KeyWords:**

portName: string

distanceMM: float (位置寸动距离，unit:mm)

distanceANG: float (关节/姿态寸动距离，unit:°度)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetInchParam",
    "params": {
        "portName": "COM4",
        "distanceMM": 0,
        "distanceANG": 0
    }
}
```
