# 4.1.1 SearchDobot

Check the current status of the devicerequest params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| filter | string | yes | filter connection mode（such as the name of 
      the serial port） |

response result
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| status | string | yes | current status of the device（connected 
      ，unconnected，occupied，unknown） |
| description | string | yes | device 
description |


KeyWords:

portName: string 

status: string (connected, unconnected, occupied, unknown)

filter: string (separate with ' ')



request:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SearchDobot",
    "params": {
        "filter": "Bluetooth VM-3..."
    }
}
```



response:

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