# 3.14.1 SetCPParams

KeyWords:

portName: string

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float (isRealTimeTrack = false)

*period: float (isRealTimeTrack = true)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetCPParams",
    "params": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100,
        "isQueued": false
    }
}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetCPParams",
    "params": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": true,
        "period": 20,
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com