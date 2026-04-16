# 4.8.3 SetEndEffectorType

Set end fitting type


 request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| type | int | yes | end fitting type (0: no fitting, 1: suction 
      cup fitting, 2: claw fitting, 3: pen fitting) |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result |






KeyWords:

portName: string

type: int (0:None 1:SucktionCup 2:Gripper 3:Pen)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetEndEffectorType",
    "params": {
        "portName": "COM4",
        "type": 1,
        "isQueued": false
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com