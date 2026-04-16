# 4.4.2 GetArmSpeedRatio

Get manipulator speed



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| type | int | yes | sport type (0: jog speed, 1: point-to-point 
      motion 
speed) |





response result




| field | type | required | explain |
| --- | --- | --- | --- |
| type | int | yes | communication port of the device |
| value | int | yes | movement speed |





KeyWords:

portName: string

type : int (0:JOG 1:PTP)

value: int (0~100 unit:%)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetArmSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "type": 1,        "value": 0    }
}
```


Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com