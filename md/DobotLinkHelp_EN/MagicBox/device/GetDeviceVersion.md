# 5.2.4 GetDeviceVersion

Get device version number



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| deviceName | string | yes | equipment name |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| majorVersion | int | yes | major version number |
| minorVersion | int | yes | minor version number |
| revision | int | yes | revision number |
| hwVersion | int | yes | hardware version 
number |




KeyWords:

portName: string

majorVersion: int

minorVersion: int

revision: int

hwVersion: int

deviceName: device name



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetDeviceVersion",
    "params": {
        "portName": "COM4",
        "deviceName":"MagicBox"
    }
}
```



OUTPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "majorVersion": 2,
        "minorVersion": 0,
        "revision": 0,
        "hwVersion": 6 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com