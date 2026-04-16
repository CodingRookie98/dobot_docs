### 7.7.5 SetCalibrateLeftRightHand

**KeyWords:**

portName: string

data: object

left/right: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCalibrateLeftRightHand",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "left" : 1.1,
            "right" : 1.1
        }
    }
}
```
