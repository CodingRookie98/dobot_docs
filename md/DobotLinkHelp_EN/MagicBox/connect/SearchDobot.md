# 5.1.1 SearchDobot

View the current status of the devicerequest params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| filter | string | yes | Filter connection mode (such as serial port 
      name) |

response result
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the
     
     
     
     
          
    
device |
| status | string | yes | Current state of the device (connected, 
      unconnected, occupied, unknown) |
| description | string | yes | Device 
description |


KeyWords:

portName: string 

status: string (connected, unconnected, occupied, unknown)

*filter: string (separate with ' ')



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SearchDobot",
    "params": {
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
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com