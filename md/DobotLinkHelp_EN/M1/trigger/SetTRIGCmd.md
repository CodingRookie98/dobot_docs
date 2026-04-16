# 6.20.1 SetTRIGCmd

KeyWords:

portName: string

port: int 

condition: int (0:equal 1:unequal, 0:less 1:less or equal)

mode: int (0:level 1:AD)

threshold: int (0~1, 0~4095)

*isQueued: bool (default:false)

*isWaitForFinish: bool (default:true)

*timeout: int (default:10000)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetTRIGCmd",
    "params": {
        "portName": "COM4",
        'port': 5,
        'condition': 1,
        'mode': 1,
        'threshold': 1000,
        'isQueued': true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com