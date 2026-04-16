# 3.11.6 SetPTPJointParams

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
    "method": "dobotlink.Magician.SetPTPJointParams",
    "params": {
        "portName": "COM4",
        "velocity": [200, 200, 200, 200],
        "acceleration": [200, 200, 200, 200],
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com