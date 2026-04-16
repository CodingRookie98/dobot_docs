# 6.2.5 GetDeviceVersion

KeyWords:

portName: string

type: int

majorVersion: int

minorVersion: int

revision: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetDeviceVersion",
    "params": {
        "portName": "COM4",
        "type": 2
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
        "type": 2,
        "majorVersion": 3,
        "minorVersion": 6,
        "revision": 14
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com