# 4.3.5 QueuedCmdStopDownload

Complete instruction queue Download

request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |

response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result |






KeyWords:

portName: string



INPUT:

```json

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.QueuedCmdStopDownload",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:

```json


```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com