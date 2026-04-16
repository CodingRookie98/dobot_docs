### 6.13.7 SetPTPCommonParams

**KeyWords:**

portName: string

velocityRatio: float

accelerationRatio: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetPTPCommonParams",
    "params": {
        "portName": "COM4",
        "velocityRatio": 100,
        "accelerationRatio": 100,
        "isQueued": false
    }
}
```
