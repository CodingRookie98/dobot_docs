# 3.14.2 GetCPParams

KeyWords:

portName: string

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float (isRealTimeTrack = false)

*period: float (isRealTimeTrack = true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetCPParams",
    "params": {
        "portName": "COM4"
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
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100
    }
}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": true,
        "period": 20
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com