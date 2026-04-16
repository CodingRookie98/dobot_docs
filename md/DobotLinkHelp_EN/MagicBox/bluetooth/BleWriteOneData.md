# 5.11.6 BleWriteOneData

Bluetooth data transmission is only applicable to Bluetooth host mode, and only one data is sent





request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| data | string | yes | data 
content |









response result




| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |





KeyWords:

portName: string

data: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleWriteOneData",
    "params": {
        "portName": "COM4" ,
        "data": "1"
    }
}
```

OUTPUT：

```json

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```

```json

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com