### 3.12.10 SetEMotorS

**KeyWords:**

portName: string

index: int (0~1)

enable: bool

speed: int (unit:pulse/sec)

distance: int (unit:pulse)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetEMotorS",
    "params": {
        "portName": "COM4",
        "index": 1,
        "enable": true,
        "speed": 250,
        "distance": 200,
        "isQueued": false
    }
}
```
