### 3.12.6 GetIOPWM

**KeyWords:**

portName: string

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetIOPWM",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```
