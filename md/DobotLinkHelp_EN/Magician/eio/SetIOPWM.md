# 3.12.5 SetIOPWM

KeyWords:

portName: string

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetIOPWM",
    "params": {
        "portName": "COM4",
        "port": 1,
        "frequency": 10.2,
        "dutyCycle": 30.0,
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com