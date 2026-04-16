# 3.15.3 SetARCCmd

KeyWords:

portName: string

cirPoint: object (float)

toPoint: object (float)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetARCCmd",
    "params": {
        "portName": "COM4",
        "cirPoint": {
            "x": 10,
            "y": 10,
            "z": 10,
            "r": 10,
        },
        "toPoint": {
            "x": 210,
            "y": 120,
            "z": 10,
            "r": 0,
        },
        "isQueued": true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com