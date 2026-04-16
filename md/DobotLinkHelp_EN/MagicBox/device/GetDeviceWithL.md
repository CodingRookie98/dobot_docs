# 5.2.6 GetDeviceWithL

Get device slide status


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| isEnabled | bool | yes | enabled (true: enabled; false: not 
    enabled) |








KeyWords:

portName: string

isEnabled: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetDeviceWithL",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT：

```json

```json


{    "id": 1,    "jsonrpc": "2.0",    "result": {        "isEnabled": true    }}
    

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com