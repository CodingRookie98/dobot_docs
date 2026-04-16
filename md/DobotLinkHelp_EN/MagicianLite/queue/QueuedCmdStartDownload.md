# 4.3.4 QueuedCmdStartDownload

Start command queue Download

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| totalLoop | int | yes | t |
| linePerLoop | int | yes | number of cycles per statement |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result |






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
    "method": "dobotlink.MagicianLite.QueuedCmdStartDownload",
    "params": {
        "portName": "COM4",
        "totalLoop": 1,
        "linePerLoop": 1
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com