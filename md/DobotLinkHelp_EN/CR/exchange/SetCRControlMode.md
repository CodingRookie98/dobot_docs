# 7.3.5 SetCRControlMode

KeyWords:

portName: string

data: object

controlMode: string ('disable', 'enable', 'drag')



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCRControlMode",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "controlMode": "disable"/"enable"/"drag"
        }
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com