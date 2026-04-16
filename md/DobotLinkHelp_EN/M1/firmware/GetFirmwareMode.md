# 6.23.5 GetFirmwareMode

KeyWords:

portName: string

firmwareMode: int(0:INVALID_MODE 1:DOBOT_MODE 2:PRINTING_MODE 3:OFFLINE_MODE 4:MTEST_MODE 5:BROKEN_MODE)

ctrl: int 



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetFirmwareMode",
    "params": {
        "portName": "COM4"
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com