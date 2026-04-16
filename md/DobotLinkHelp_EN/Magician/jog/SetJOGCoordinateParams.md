# 3.10.3 SetJOGCoordinateParams

KeyWords:

portName: string

velocity: array(float)

acceleration: array(float)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetJOGCoordinateParams",
    "params": {
        "portName": "COM4",
        "velocity": [60, 60, 60, 60],
        "acceleration": [60, 60, 60, 60],
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com