# 5.7.5 SetIOPWM

Set I / O PWM output





request params


| field | type | requried | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | EIO address（0~25） |
| frequency | float | yes | PWM frequency(10Hz~1MHz) |
| dutyCycle | float | yes | PWM Duty cycle 0~100 |
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

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetIOPWM",
    "params": {
        "portName": "COM4",
        "port": 1,
        "frequency": 10.2,
        "dutyCycle": 30.0,
        "isQueued": false
    }
}
```





OUTPUT：

```json

```json


{    "id": 1,    "jsonrpc": "2.0".
    "result": true }


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com