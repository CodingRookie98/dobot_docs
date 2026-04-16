# 5.11.4 BleConnect

Setting Bluetooth connection is only applicable to the Bluetooth host mode. Bluetooth will scan and connect the slave with the specified name



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| time | int | yes | Connection timeout，unit:second |
| name | string | yes | string |







response result




| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |





KeyWords:

portName: string

time: int，Connection timeout，unit:second

name: string, the length is within 14 bytes, and the insufficient part is filled with 0



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleConnect",
    "params": {
        "portName": "COM4" ,
        "time": 100, 
        "name": "string"
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com