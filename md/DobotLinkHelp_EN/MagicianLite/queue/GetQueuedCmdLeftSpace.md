# 4.3.7 GetQueuedCmdLeftSpace

Gets the remaining space of the instruction queue
request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| leftSpace | int | yes | amount of space left |






KeyWords:

portName: string

leftSpace: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetQueuedCmdLeftSpace",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "leftSpace": 32    }   
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com