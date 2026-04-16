# 5.10.1 DownloadProgram

Download the offline script to the USB flash drive of box





request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| code | string | yes | file content in Base64 transcoding utf8 
      encoding format |
| fileName | string | yes | file name |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |








KeyWords:

portName: string

code: string，file content in Base64 transcoding utf8 encoding format

*fileName: string (default:temp)，file name

INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.DownloadProgram",
    "params": {
        "portName": "COM4",
        "code": "# -*- coding: UTF-8 -*-\n ...... ",
        "fileName": "dobot_scratch.py"
    }
}
```
OUTPUT:
```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com