### 6.14.3 SetMotivateCmd

**KeyWords:**

portName: string

q1,q2: float

dq1,dq2: float

ddq1,ddq2: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:10000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetMotivateCmd",
    "params": {
        "portName": "COM4",
        "q1": 1.0,
        "q2": 2.0,
        "dq1": 1.0,
        "dq2": 2.0,
        "ddq1": 1.0,
        "ddq2": 2.0,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
