### 3.11.1 SetPTPCmd

**KeyWords:**

portName: string

ptpMode: int(0~9)

x: float

y: float

z: float

r: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:5000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPCmd",
    "params": {
        "portName": "COM4",
        "ptpMode": 1,
        "x": 210,
        "y": 100,
        "z": 10,
        "r": 0,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
