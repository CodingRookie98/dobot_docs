### 3.11.8 SetPTPCoordinateParams

**KeyWords:**

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPCoordinateParams",
    "params": {
        "portName": "COM4",
        "xyzVelocity": 200,
        "rVelocity": 100,
        "xyzAcceleration": 200,
        "rAcceleration": 100,
        "isQueued": false
    }
}
```
