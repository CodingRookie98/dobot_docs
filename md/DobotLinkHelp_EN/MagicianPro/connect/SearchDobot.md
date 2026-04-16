# 8.1.1 SearchDobot

KeyWords:

portName: string

status: string (connected, unconnected)

version: string 版本号

type: string 设备类型



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SearchDobot"
}
```

```json

 



OUTPUT:
 


```json

```json
{
    "id": 1,
    "jsonrpc": "2.0", 
    "result": [{ 
        "portName": "192.168.1.6", 
        "status": "connected",
        "version": "1.3.0",
        "type": "MG400"
    }, {
        "portName": "192.168.9.1", 
        "status": "unconnected", 
        "version": "2.3.0", 
        "type": "M1Pro"
    }]
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)