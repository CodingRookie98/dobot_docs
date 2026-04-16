### 3.11.3 SetPTPWithLCmd

**KeyWords:**

portName: string

ptpMode: int(0~9)

x: float

y: float

z: float

r: float

l: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPWithLCmd",
    "params": {
        "portName": "COM4",
        "ptpMode": 1,
        "x": 210,
        "y": 100,
        "z": 10,
        "r": 0,
        "l": 200,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
