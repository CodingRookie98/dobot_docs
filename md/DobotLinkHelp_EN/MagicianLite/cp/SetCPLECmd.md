# 4.13.4 SetCPLECmd

Perform continuous track gray engraving function


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| cpMode | int | yes | CP mode (0: relative mode 1: absolute mode) |
| x | float | yes | x coordinate increment / x axis coordinate |
| y | float | yes | y coordinate increment / y axis coordinate |
| z | float | yes | z coordinate increment / z axis coordinate |
| power | float | yes | laser power |
| isQueued | bool | yes | Queued instructions (true: instructions are 
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

cpMode: int (0~1)

x: float

y: float

z: float

power: float

*isQueued: bool (default:true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCPLECmd",
    "params": {
        "portName": "COM4",
        "cpMode": 0,
        "x": 20.0,
        "y": 5.0,
        "z": 1.0,
        "power": 20.0,
        "isQueued": true
    }
}
```



OUTPUT:

```json

```json

{
    "id": 1,     "jsonrpc": "2.0",    "result": true
 
}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com