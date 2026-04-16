# 5.11.3 GetBleInf

Get Bluetooth master-slave mode




request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| name | string | yes | String, the length is within 14 bytes, and the 
      insufficient part is filled with 0 |





KeyWords:

portName: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetBleInf",
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
    "method": "dobotlink.MagicBox.GetBleInf",
    "params": {
        "name": "string" 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com