### 6.1.3 DisconnectDobot

**KeyWords:**

portName: string

*queueStop: bool (default:true)

*queueClear: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.DisconnectDobot",
    "params": {
        "portName": "COM4",
        "queueStop": true,
        "queueClear": true
    }
}
```
