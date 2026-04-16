# 5.11.9 BleWriteMeshData

Bluetooth networking mode data transmission 



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| devID | int | yes | sender ID |
| data | string | yes | data 
content |







 response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |







KeyWords:

portName: string

devID: int，sender ID

data: string，data content



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleWriteMeshData",
    "params": {
        "portName": "COM4",
        "devID": 123,
        "data": "string" 
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com