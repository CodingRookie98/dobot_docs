### 9.1.3 SearchDobot

**KeyWords:**

portName: string

status: string (connected, unconnected, occupied, unknown)

filter: string (separate with ' ')

connectCheck: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SearchDobot",
    "params": {
        "connectCheck": false,
        "filter": "Bluetooth VM-3..."
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": [{
        "portName": "COM3",
        "status": "unconnected",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }, {
        "portName": "COM15",
        "status": "occupied",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }]
}
```
