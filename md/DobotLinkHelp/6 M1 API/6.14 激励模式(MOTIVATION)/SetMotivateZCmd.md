### 6.14.4 SetMotivateZCmd

**KeyWords:**

portName: string

qz, dqz, ddqz: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:10000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetMotivateZCmd",
    "params": {
        "portName": "COM4",
        "qz": 1.0,
        "dqz": 2.0,
        "ddqz": 1.0,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
