# 4.7.1 SetHOMEParams

Set zero return parameter

request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| x | float | yes | Current x position |
| y | float | yes | Current y position |
| z | float | yes | Current z position |
| r | float | yes | Current r position |
| isQueued | bool | yes | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: false |

response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result |




KeyWords:

portName: string

x: float

y: float

z: float

r: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetHOMEParams",
    "params": {
        "portName": "COM4",
        "x": 20.65,
        "y": 5.84,
        "z": 2.36,
        "r": 0.0,
        "isQueued": false
    }
}
```



OUTPUT:

```json

```json

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true   
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com