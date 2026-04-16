# 7.4.11 SetPlaybackArch

KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetPlaybackArch",
    "params": {
        "portName": "192.168.5.1",
        "data": [{
            "enable": true,
            "params": {
                "startHeight": 10,
                "endHeight": 15,
                "zLimit": 200
            }
        }, {
            "enable": false,
            "params": {
                "startHeight": 11,
                "endHeight": 20,
                "zLimit": 200
            }
        }]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com