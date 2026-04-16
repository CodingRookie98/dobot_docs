### 6.1.1 SearchDobot

**KeyWords:**

portName: string

status: string (connected, unconnected, occupied, unknown)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SearchDobot"
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": [{
        "portName": "192.168.1.103",
        "status": "unconnected",
        "description": "dobotM1_"
    }, {
        "portName": "COM15",
        "status": "occupied",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }]
}
```
