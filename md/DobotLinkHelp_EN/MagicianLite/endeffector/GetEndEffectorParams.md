# 4.8.2 GetEndEffectorParams

Get end effector parameters


request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |

response result



| field | type | required | explain |
| --- | --- | --- | --- |
| xOffset | int | yes | End x-axis length |
| yOffset | int | yes | End y-axis length |
| zOffset | int | yes | End z-axis 
length |









KeyWords:

portName: string

xOffset: float

yOffset: float

zOffset: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorParams",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "xOffset": 57,        "yOffset": 0,        "zOffset": 0    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com