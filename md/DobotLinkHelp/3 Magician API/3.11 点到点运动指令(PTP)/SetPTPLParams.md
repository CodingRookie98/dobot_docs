### 3.11.14 SetPTPLParams

**KeyWords:**

portName: string

velocity: float

acceleration: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPLParams",
    "params": {
        "portName": "COM4",
        "velocity": 200,
        "acceleration": 200,
        "isQueued": false
    }
}
```
