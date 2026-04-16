# 4.7.3 SetHOMECmd

Execute the zero return command

request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) |
| isWaitForFinish | bool | no | Whether to wait for the instruction to 
      complete (true: wait for the instruction to complete before returning; 
      false: return immediately after receiving the instruction) |
| timeout | int | no | Motion timeout, 8 seconds by 
  default |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result |






KeyWords:

portName: string

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:8000)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetHOMECmd",
    "params": {
        "portName": "COM4",
        "isQueued": true,
        "isWaitForFinish": true
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