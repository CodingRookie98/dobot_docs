### 3.4.5 SetLSpeedRatio

**KeyWords:**

portName: string

type: int (0:JOG 1:PTP)

value: int (0~100 unit:%)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetLSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1,
        "value": 50,
        "isQueued": false
    }
}
```
