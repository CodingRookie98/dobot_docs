### 3.14.4 SetCPLECmd

**KeyWords:**

portName: string

cpMode: int (0~1)

x: float

y: float

z: float

power: float

*isQueued: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetCPLECmd",
    "params": {
        "portName": "COM4",
        "cpMode": 0,
        "x": 20.0,
        "y": 5.0,
        "z": 1.0,
        "power": 20.0,
        "isQueued": true
    }
}
```
