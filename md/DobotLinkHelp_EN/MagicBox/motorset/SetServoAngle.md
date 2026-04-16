# 5.4.1 SetServoAngle

Set the angle of the steering gear



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| index | int | yes | steering gear serial number: port number 0-5 |
| value | float | yes | angle value (+ / - 180) |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
      false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| angle | int | yes | angle value (+ / - 
      180) |
| index | int | yes | steering gear serial number: port number 
0-5 |






KeyWords:

portName: string

index: int

value: float (+/-180)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetServoAngle",
    "params": {
        "portName": "COM4",
        "index": 2,
        "value": 60,
        "isQueued": false
    }
}
```



OUTPUT:

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "angle": 60,        "index": 2    }}
```json
    

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com