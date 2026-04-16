### 3.9.3 SetEndEffectorType

**KeyWords:**

portName: string

type: int (0:None 1:SucktionCup 2:Gripper 3:Pen)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetEndEffectorType",
    "params": {
        "portName": "COM4",
        "type": 1,
        "isQueued": false
    }
}
```
