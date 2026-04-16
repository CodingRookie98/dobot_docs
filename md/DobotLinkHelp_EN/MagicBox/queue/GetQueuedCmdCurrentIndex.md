# 5.3.6 GetQueuedCmdCurrentIndex

Get instruction queue index


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |




response result


| field | type | required | explain |
| --- | --- | --- | --- |
| queuedCmdIndex | int | yes | Queue 
      command index |






KeyWords:

portName: string

queuedCmdIndex: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetQueuedCmdCurrentIndex",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {
        "queuedCmdIndex": 56    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com