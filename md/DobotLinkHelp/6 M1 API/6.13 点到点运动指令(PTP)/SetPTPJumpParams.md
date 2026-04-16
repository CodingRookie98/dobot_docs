### 6.13.5 SetPTPJumpParams

**KeyWords:**

portName: string

isUsingZLimit: true

zLimit: float

jumpHeight: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetPTPJumpParams",
    "params": {
        "portName": "COM4",
        "isUsingZLimit": true,
        "zLimit": 100,
        "jumpHeight": 20,
        "isQueued": false
    }
}
```
