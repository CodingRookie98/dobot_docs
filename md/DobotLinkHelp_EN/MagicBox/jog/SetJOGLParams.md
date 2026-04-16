# 5.8.2 SetJOGLParams

Set the jog parameters of slide rail L



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| velocity | float | yes | slide joint speed |
| acceleration | float | yes | acceleration of slide rail joint |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
      false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation
     
     
     
     
         
         
         
         
    
failed) |








KeyWords:

portName: string

velocity: float

acceleration: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetJOGLParams",
    "params": {
        "portName": "COM4",
        "velocity": 60,
        "acceleration": 60,
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com