### 3.4.1 SetArmSpeedRatio

**KeyWords:**

portName: string

type: int (0:JOG 1:PTP 2:CP 3:ARC)

value: int (0~100 unit:%)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetArmSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1,
        "value": 50,
        "isQueued": false
    }
}
```
