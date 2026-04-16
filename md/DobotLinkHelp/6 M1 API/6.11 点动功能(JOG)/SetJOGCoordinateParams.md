### 6.11.3 SetJOGCoordinateParams

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetJOGCoordinateParams",
    "params": {
        "portName": "COM4",
        "velocity": [60, 60, 60, 60],
        "acceleration": [60, 60, 60, 60],
        "isQueued": false
    }
}
```
