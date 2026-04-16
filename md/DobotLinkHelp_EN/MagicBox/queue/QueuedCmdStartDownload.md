# 5.3.4 QueuedCmdStartDownload

Start command queue Download

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| totalLoop | int | yes | total number of cycles |
| linePerLoop | int | yes | Number of cycles per 
statement |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |




KeyWords:

portName: string

totalLoop: int

linePerLoop: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.QueuedCmdStartDownload",
    "params": {
        "portName": "COM4",
        "totalLoop": 10,
        "linePerLoop": 20
    }
}
```

OUTPUT:

```json

 
```json
{
    "id": 1    "jsonrpc": "2.0"    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com