### 3.10.9 SetJOGCmd

**KeyWords:**

portName: string

isJoint: bool

cmd: int (0:stop X:1,2 Y:3,4 Z:5,6 R:7,8 L:9,10(isJoint = true))

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetJOGCmd",
    "params": {
        "portName": "COM4",
        "isJoint": false,
        "cmd": 2,
        "isQueued": false
    }
}
```
