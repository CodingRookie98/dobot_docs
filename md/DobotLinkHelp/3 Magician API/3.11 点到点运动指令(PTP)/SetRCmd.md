### 3.11.2 SetRCmd

**KeyWords:**

portName: string

r: int

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:5000)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetRCmd",
    "params": {
        "portName": "COM4",
        "r": 100
    }
}
```
