### 3.12.5 SetIOPWM

**KeyWords:**

portName: string

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetIOPWM",
    "params": {
        "portName": "COM4",
        "port": 1,
        "frequency": 10.2,
        "dutyCycle": 30.0,
        "isQueued": false
    }
}
```
