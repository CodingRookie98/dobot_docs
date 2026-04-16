# 5.8.1 SetJOGCmd

Executive inching kinetic energy



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |
| isJoint | bool | yes | inching mode (0: coordinate axis jogging, 
      1: Joint inching) |
| cmd | int | yes | jog command (value range 0 ~ 8) |
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

isJoint: bool

cmd: int (L:9,10)

*isQueued: bool (default:false)



INPUT:



```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetJOGCmd",
    "params": {
        "portName": "COM4",
        "isJoint": true,
        "cmd": 9,
        "isQueued": false
    }
}
```



OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com