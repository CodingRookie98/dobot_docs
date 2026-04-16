### 6.25.1 SetRebootEncoderICPVL

**KeyWords:**

portName: string

jointNumber: float (1.0:joint1 2.0:joint2 3.0:joint3 4.0:joint4)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetRebootEncoderICPVL",
    "params": {
        "portName": "COM4",
        "jointNumber": 1.0
    }
}
```
