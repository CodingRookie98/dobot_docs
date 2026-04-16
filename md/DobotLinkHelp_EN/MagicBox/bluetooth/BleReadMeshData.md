# 5.11.8 BleReadMeshData

Bluetooth networking mode data reception 





request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| state | int | yes | 0 - receive succeeded, others - receive 
      failed |
| devID | int | yes | sender ID |
| data | string | yes | data 
content |







KeyWords:

portName: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleReadMeshData",
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
    "result":
    { 
       "state":0, //0 - receive succeeded, others - receive failed 
       "devID": 123 , //senderID 
       "data": "string" //data     content
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com