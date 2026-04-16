### 3.7.3 SetHOMECmd

**KeyWords:**

portName: string

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:25000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetHOMECmd",
    "params": {
        "portName": "COM4",
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
