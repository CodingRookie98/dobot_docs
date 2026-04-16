# 4.10.7 SetPTPJumpParams

Set door mode point parameters



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| zLimit | float | yes | maximum lifting height limit of door mode 
      movement |
| jumpHeight | float | yes | lifting distance of door mode 
movement |
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

zLimit: float

jumpHeight: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetPTPJumpParams",
    "params": {
        "portName": "COM4",
        "zLimit": 100,
        "jumpHeight": 20,
        "isQueued": false
    }
}
```



OUTPUT：

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```json
    

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com