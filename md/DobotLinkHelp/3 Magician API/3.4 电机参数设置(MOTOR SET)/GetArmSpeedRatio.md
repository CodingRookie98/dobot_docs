### 3.4.2 GetArmSpeedRatio

**KeyWords:**

portName: string

type: int (0:JOG 1:PTP 2:CP 3:ARC)

value: int (0~100 unit:%)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetArmSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1
    }
}
```
