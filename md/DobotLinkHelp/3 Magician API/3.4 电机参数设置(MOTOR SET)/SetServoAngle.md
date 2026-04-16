### 3.4.3 SetServoAngle

**KeyWords:**

portName: string

index: int

value: float (+/-180)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetServoAngle",
    "params": {
        "portName": "COM4",
        "index": 2,
        "value": 60,
        "isQueued": false
    }
}
```
