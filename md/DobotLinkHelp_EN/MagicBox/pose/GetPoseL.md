# 5.5.1 GetPoseL

Acquire real-time position and attitude of slide rail


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| positionL | float | yes | slide rail position |










KeyWords:

portName: string

positionL: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetPoseL",
    "params": {
        "portName": "COM4",
    }
}
```





OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "positionL": 0    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com