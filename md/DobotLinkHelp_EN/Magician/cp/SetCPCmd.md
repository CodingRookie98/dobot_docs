# 3.14.3 SetCPCmd

KeyWords:

portName: string

cpMode: int (0~1)

x: float

y: float

z: float

power: float

*isQueued: bool (default:true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetCPCmd",
    "params": {
        "portName": "COM4",
        "cpMode": 0,
        "x": 20.0,
        "y": 5.0,
        "z": 1.0,
        "power": 20.0,
        "isQueued": true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com