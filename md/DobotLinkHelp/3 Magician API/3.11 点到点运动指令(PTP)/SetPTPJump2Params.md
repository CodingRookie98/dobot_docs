### 3.11.16 SetPTPJump2Params

**KeyWords:**

portName: string

zLimit: float

startJumpHeight: float

endJumpHeight: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPJump2Params",
    "params": {
        "portName": "COM4",
        "zLimit": 100,
        "startJumpHeight": 20,
        "endJumpHeight": 20,
        "isQueued": false
    }
}
```
