### 6.17.1 SetARCParams

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
    "method": "dobotlink.M1.SetARCParams",
    "params": {
        "portName": "COM4",
        "xyzVelocity": 200,
        "rVelocity": 200,
        "xyzAcceleration": 200,
        "rAcceleration": 200,
        "isQueued": false
    }
}
```
