# 4.14.4 SetCircleCmd

Circular motion


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| cirPoint | object | yes | coordinates of any point in the arc |
| toPoint | object | yes | arc end point coordinates |
| isQueued | bool | no | Queued instructions (true: instructions are queued 
      for execution, false: interrupt the currently executed task and insert it 
      directly for execution) default: 
      false |
| isWaitForFinish | bool | no | Wait for completion (default: true) |
| timeout | int | no | run timeout 
(60000)f |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |










KeyWords:

portName: string

cirPoint: object (float)

toPoint: object (float)

count: int

*isQueued: bool (default:false)

*isWaitForFinish: bool (default:true)

*timeout: int (default:60000)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCircleCmd",
    "params": {
        "portName": "COM4",
        "cirPoint": {
            "x": 10,
            "y": 10,
            "z": 10,
            "r": 10
        },
        "toPoint": {
            "x": 210,
            "y": 120,
            "z": 10,
            "r": 0
        },
        "count": 10,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```

OUTPUT：

```json

```json

{
    "id": 1,     "jsonrpc": "2.0",    "result": true} 


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com