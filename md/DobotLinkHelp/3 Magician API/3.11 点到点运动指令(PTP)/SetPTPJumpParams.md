### 3.11.10 SetPTPJumpParams

**KeyWords:**

portName: string

zLimit: float

jumpHeight: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPJumpParams",
    "params": {
        "portName": "COM4",
        "zLimit": 100,
        "jumpHeight": 20,
        "isQueued": false
    }
}
```
