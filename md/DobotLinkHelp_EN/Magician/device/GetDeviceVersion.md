# 3.2.5 GetDeviceVersion

KeyWords:

portName: string

majorVersion: int

minorVersion: int

revision: int

hwVersion: int

deviceName: 设备名称



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetDeviceVersion",
    "params": {
        "portName": "COM4",
        "deviceName":"Magician"
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
        "majorVersion": 3,
        "minorVersion": 6,
        "revision": 14,
        "hwVersion": 1 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com