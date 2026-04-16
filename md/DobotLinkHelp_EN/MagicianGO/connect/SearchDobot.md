# 9.1.3 SearchDobot

KeyWords:

portName: string

status: string (connected, unconnected, occupied, unknown)

filter: string (separate with ' ')

connectCheck: bool



INPUT:

```json

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
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)