### 3.12.9 SetEMotor

**KeyWords:**

portName: string

index: int (0~1)

enable: bool

speed: int (unit:pulse/sec)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetEMotor",
    "params": {
        "portName": "COM4",
        "index": 1,
        "enable": true,
        "speed": 250.0,
        "isQueued": false
    }
}
```
