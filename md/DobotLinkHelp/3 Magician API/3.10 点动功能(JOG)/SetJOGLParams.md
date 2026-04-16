### 3.10.7 SetJOGLParams

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
    "method": "dobotlink.Magician.SetJOGLParams",
    "params": {
        "portName": "COM4",
        "velocity": 60,
        "acceleration": 60,
        "isQueued": false
    }
}
```
