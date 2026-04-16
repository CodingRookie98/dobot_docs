### 3.8.1 SetHHTTrigMode

**KeyWords:**

portName: string

mode: int (0:TriggeredOnKeyReleased 1:TriggeredOnPeriodicInterval)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetHHTTrigMode",
    "params": {
        "portName": "COM4",
        "mode": 1,
        "isQueued": false
    }
}
```
