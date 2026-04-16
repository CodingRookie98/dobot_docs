### 6.11.5 SetJOGCommonParams

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
    "method": "dobotlink.M1.SetJOGCommonParams",
    "params": {
        "portName": "COM4",
        "velocityRatio": 100,
        "accelerationRatio": 50,
        "isQueued": false
    }
}
```
