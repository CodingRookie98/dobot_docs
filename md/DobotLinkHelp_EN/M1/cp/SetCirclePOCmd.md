# 6.17.6 SetCirclePOCmd

KeyWords:

portName: string

x,y,z,r: float

count: int

ratio: int

port: int

level: int

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetCirclePOCmd",
    "params": {
        "portName": "COM4",
        "cirPoint": {
            "x": 10,
            "y": 10,
            "z": 10,
            "r": 10
        },
        "toPoint": {
            "x": 210,
            "y": 120,
            "z": 10,
            "r": 0
        },
        "count": 10,
        "circlePO": [{
            "ratio": 20,
            "port": 1,
            "level":2
        },{
            "ratio":30,
            "port": 1,
            "level":1
        }]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com