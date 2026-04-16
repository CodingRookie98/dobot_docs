### 6.7.1 SetHOMECmd

**KeyWords:**

portName: string

isResetPars: bool (default:false)

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:60000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetHOMECmd",
    "params": {
        "portName": "COM4",
        "isResetPars": false,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
