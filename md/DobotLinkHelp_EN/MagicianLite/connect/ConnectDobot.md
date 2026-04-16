# 4.1.2 ConnectDobot

Connect current device

request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | 是 | communication port of the 
device |

response result
| field | type | required | explain |
| --- | --- | --- | --- |
| firmwareName | string | yes | firmware name |
| firmwareVersion | string | yes | firmware version |
| productName | string | yes | device 
name |


KeyWords:

portName: string





INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.ConnectDobot",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "firmwareName": "Dobot",        "firmwareVersion": "",        "productName": ""    }}
```

```json
 

```

```json
 
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com