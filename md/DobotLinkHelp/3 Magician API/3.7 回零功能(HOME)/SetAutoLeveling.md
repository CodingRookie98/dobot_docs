### 3.7.4 SetAutoLeveling

**KeyWords:**

portName: string

enable: bool

precision: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetAutoLeveling",
    "params": {
        "portName": "COM4",
        "enable": true,
        "precision": 10.2,
        "isQueued": false
    }
}
```
