# 2.5 ShowAvailablePorts

Description: 返回当前电脑所有串口

KeyWords:

portName: string

description: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.api.ShowAvailablePorts"
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
        "description": "Arduino Uno"
    }, {
        "portName": "COM4",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }]
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com