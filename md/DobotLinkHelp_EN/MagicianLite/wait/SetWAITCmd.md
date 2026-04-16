# 4.15.1 SetWAITCmd

Execution time waiting function



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| delay | int | yes | waiting time (unit: 
ms) |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, false: 
      operation failed) |




KeyWords:

portName: string

delay: int 

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetWAITCmd",
    "params": {
        "portName": "COM4",
        "delay": 500
    }
}
```



OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com