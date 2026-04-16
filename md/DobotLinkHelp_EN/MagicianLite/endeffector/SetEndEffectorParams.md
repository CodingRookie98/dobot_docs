# 4.8.1 SetEndEffectorParams

Set end effector parameters
request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| xOffset | float | yes | End x-axis length |
| yOffset | float | yes | End y-axis length |
| zOffset | float | yes | End z-axis length |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |








KeyWords:

portName: string

xOffset: float

yOffset: float

zOffset: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetEndEffectorParams",
    "params": {
        "portName": "COM4",
        "xOffset": 57.0,
        "yOffset": 0.0,
        "zOffset": 0.0,
        "isQueued": false
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com