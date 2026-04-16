### 3.12.13 SetInfraredSensor

**KeyWords:**

portName: string

port: int (0~25)

enable: bool

version: int

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetInfraredSensor",
    "params": {
        "portName": "COM4",
        "port": 1,
        "enable": true,
        "version": 1,
        "isQueued": false
    }
}
```
