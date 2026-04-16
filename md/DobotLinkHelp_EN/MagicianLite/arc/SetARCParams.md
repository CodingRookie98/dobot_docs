# 4.14.1 SetARCParams

Set arc interpolation function parameters


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| xyzVelocity | float | yes | circular motion xyz triaxial velocity |
| rVelocity | float | yes | end rotation speed of circular motion |
| xyzAcceleration | float | yes | circular motion XYZ triaxial acceleration |
| rAcceleration | float | yes | rotation acceleration at the end of circular 
      motion |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
      false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation 
      succeeded, false: operation failed) |




KeyWords:

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetARCParams",
    "params": {
        "portName": "COM4",
        "xyzVelocity": 200,
        "rVelocity": 200,
        "xyzAcceleration": 200,
        "rAcceleration": 200,
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