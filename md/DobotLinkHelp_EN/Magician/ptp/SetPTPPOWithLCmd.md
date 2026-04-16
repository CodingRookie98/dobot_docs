# 3.11.5 SetPTPPOWithLCmd

KeyWords:

portName: string

ptpMode: int(0~9)

x: float

y: float

z: float

r: float

l: float

ratio: int

port: int

level: int

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetPTPPOWithLCmd",
    "params": {
        "portName": "COM4",
        "ptpCmd": {
            "ptpMode": 1,
            "x": 210,
            "y": 100,
            "z": 10,
            "r": 0,
            "l": 200
        },
        "poCmd": [{
            "ratio": 10,
            "address": 1,
            "level": 1
        }, {
            "ratio": 10,
            "port": 2,
            "level": 0
        }],
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com