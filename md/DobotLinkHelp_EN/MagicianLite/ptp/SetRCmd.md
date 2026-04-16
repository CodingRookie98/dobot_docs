# 4.10.2 SetRCmd

Sets the value of the R-axis



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| r | float | yes | current r position |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: false |
| isWaitForFinish | bool | no | Whether to wait for the instruction to 
      complete (true: wait for the instruction to complete before returning; 
      false: return immediately after receiving the instruction) |
| timeout | bool | no | movement timeout, default to 
5S |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |








KeyWords:

portName: string

r: int

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:5000)







INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetRCmd",
    "params": {
        "portName": "COM4",
        "r": 100
    }
}
```





```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```json


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com