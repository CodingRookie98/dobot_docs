# 3.12.10 SetEMotorS

KeyWords:

portName: string

index: int (0~1)

enable: bool

speed: int (unit:pulse/sec)

distance: int (unit:pulse)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetEMotorS",
    "params": {
        "portName": "COM4",
        "index": 1,
        "enable": true,
        "speed": 250,
        "distance": 200,
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com