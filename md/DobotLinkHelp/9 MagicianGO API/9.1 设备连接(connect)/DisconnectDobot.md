### 9.1.2 DisconnectDobot

**KeyWords:**

portName: string

*queueStop: bool (default:true)

*queueClear: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.DisconnectDobot",
    "params": {
        "portName": "COM4",
        "queueStop": true,
        "queueClear": true
    }
}
```
