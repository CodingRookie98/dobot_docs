# 5.11.7 SetBleMesh

Set the Bluetooth networking mode, and set the group ID and current device ID of the networking mode. 





request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| groupID | int | yes | Group ID |
| devID | int | yes | Device ID |







response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |







KeyWords:

portName: string

groupID: int,group ID, length 6 bytes, each number range 0-9

devID: int,device ID, length 1 byte, 0-255



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetBleMesh",
    "params": {
        "portName": "COM4" ,
        "groupID": 123465,
        "devID": 123
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com