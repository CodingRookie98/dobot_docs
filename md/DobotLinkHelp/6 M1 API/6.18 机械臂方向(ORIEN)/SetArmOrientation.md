### 6.18.1 SetArmOrientation

**KeyWords:**

portName: string

orientation: int (0:lefty 1:righty)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetArmOrientation",
    "params": {
        "portName": "COM4",
        "orientation": 0
    }
}
```
