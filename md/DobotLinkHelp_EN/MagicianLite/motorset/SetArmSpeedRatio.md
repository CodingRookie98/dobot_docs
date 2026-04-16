# 4.4.1 SetArmSpeedRatio

Set manipulator speed



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| type | int | yes | sport type (0 is jog speed, 1 is 
      point-to-point motion speed) |
| value | int | yes | speed value of manipulator |
| isQueued | bool | yes | queue instruction（true：instruction queuing 
      execution，false：interrupt the current task and insert it 
      directly |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result |






KeyWords:

portName: string

type : int (0:JOG 1:PTP)

value: int (0~100 unit:%)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetArmSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1,
        "value": 50,
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