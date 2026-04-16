### 3.12.3 SetIODO

**KeyWords:**

portName: string

port: int (0~25)

level: int (0~1)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetIODO",
    "params": {
        "portName": "COM4",
        "port": 1,
        "level": 1,
        "isQueued": false
    }
}
```
