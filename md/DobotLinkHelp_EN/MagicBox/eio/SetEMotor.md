# 5.7.9 SetEMotor

Set extended Motor Interface



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| index | int | yes | value range 0 / 1 (0-stepper1, 1-stepper2) |
| enable | bool | yes | motor control enable (false: not enabled, 
      true: enabled) |
| speed | int | yes | motor control speed (unit: number of pulses 
      per second) |
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

index: int (0~1)

enable: bool

speed: int (unit:pulse/sec)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetEMotor",
    "params": {
        "portName": "COM4",
        "index": 1,
        "enable": true,
        "speed": 250.0,
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