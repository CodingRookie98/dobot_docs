### 6.5.1 SetUserCoordinate

**KeyWords:**

portName: string

x: float

y: float

z: float

r: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetUserCoordinate",
    "params": {
        "portName": "COM4",
        "x": 200.0,
        "y": 150.0,
        "z": 20.0,
        "r": 0.0
    }
}
```
