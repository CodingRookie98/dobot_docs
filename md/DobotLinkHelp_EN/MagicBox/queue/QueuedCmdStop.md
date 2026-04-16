# 5.3.2 QueuedCmdStop

Stop instruction queue


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| forceStop | bool | yes | forced 
      stop queue (true: open forced stop queue, false: close forced stop 
      queue) |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |






KeyWords:

portName: string

*forceStop: bool (default: false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.QueuedCmdStop",
    "params": {
        "portName": "COM4",
        "forceStop": false
     }
}
```

 OUTPUT:

```json
{   "id": 1,    "jsonrpc": "2.0",
    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com