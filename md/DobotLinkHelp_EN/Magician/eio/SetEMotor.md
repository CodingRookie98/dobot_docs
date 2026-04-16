# 3.12.9 SetEMotor

KeyWords:

portName: string

index: int (0~1)

enable: bool

speed: int (unit:pulse/sec)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetEMotor",
    "params": {
        "portName": "COM4",
        "index": 1,
        "enable": true,
        "speed": 250.0,
        "isQueued": false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com