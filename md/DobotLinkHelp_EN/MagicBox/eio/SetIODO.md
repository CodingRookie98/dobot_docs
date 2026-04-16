# 5.7.3 SetIODO

Set I / O port output level





 request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | EIO address（0~25） |
| level | int | yes | output level (0: low level, 1: high level) |
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

level: int (0~1)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetIODO",
    "params": {
        "portName": "COM4",
        "port": 1,
        "level": 1,
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com