# 5.11.5 BleReadOneData

Bluetooth data reception, only applicable to Bluetooth host mode, only one data is received





request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |







response result




| field | type | required | explain |
| --- | --- | --- | --- |
| data | int | yes | data 
content |





KeyWords:

portName: string

data: int,data content



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleReadOneData",
    "params": {
        "portName": "COM4" 
    }
}
```

OUTPUT：

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleReadOneData",
    "params": {
        "data": 1 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com