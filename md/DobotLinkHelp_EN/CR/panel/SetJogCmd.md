# 7.6.4 SetJogCmd

KeyWords:

portName: string

data: object

posBtns: array(bool) ([x, y, z, a, b, c])

negBtns: array(bool) ([x, y, z, a, b, c])



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetJogCmd",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "posBtns": [true, false, false, false, false, false],
            "negBtns": [false, false, false, false, false, false]
        }    
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com