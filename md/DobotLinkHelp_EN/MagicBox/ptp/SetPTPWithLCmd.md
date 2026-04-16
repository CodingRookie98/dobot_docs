# 5.6.1 SetPTPWithLCmd

Perform the point position function with slide rail


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| l | float | yes | s |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
      false |
| isWaitForFinish | bool | no | whether to wait for completion (true: Yes, 
      false: no) |







 response result

| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: setting succeeded, 
      false: setting failed) |






KeyWords:

portName: string

l: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetPTPWithLCmd",
    "params": {
        "portName": "COM4",
        "l": 200,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com