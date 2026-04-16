### 6.12.4 GetInchParam

**KeyWords:**

portName: string

distanceMM: float (位置寸动距离，unit:mm)

distanceANG: float (关节/姿态寸动距离，unit:°度)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetInchParam",
    "params": {
        "portName": "COM4"
    }
}
```
