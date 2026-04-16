### 3.12.1 SetIOMultiplexing

**KeyWords:**

portName: string

port: int (0~25)

multiplex: int (0~6)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetIOMultiplexing",
    "params": {
        "portName": "COM4",
        "port": 1,
        "multiplex": 1,
        "isQueued": false
    }
}
```
