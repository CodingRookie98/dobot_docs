# 6.13.9 SetPTPCmd

KeyWords:

portName: string

ptpMode: int(0~9)

x: float

y: float

z: float

r: float

*isQueued: bool (default:true)

*isWaitForFinish: bool (default:true)

*timeout: int (default:10000)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetPTPCmd",
    "params": {
        "portName": "COM4",
        "ptpMode": 1,
        "x": 210,
        "y": 100,
        "z": 10,
        "r": 0,
        "isQueued": true,
        "isWaitForFinish": true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com