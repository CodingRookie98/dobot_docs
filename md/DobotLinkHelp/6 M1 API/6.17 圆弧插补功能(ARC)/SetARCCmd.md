### 6.17.3 SetARCCmd

**KeyWords:**

portName: string

cirPoint: object (float)

toPoint: object (float)

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:60000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetARCCmd",
    "params": {
        "portName": "COM4",
        "cirPoint": {
            "x": 10,
            "y": 10,
            "z": 10,
            "r": 10
        },
        "toPoint": {
            "x": 210,
            "y": 120,
            "z": 10,
            "r": 0
        },
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
