# 7.3.2 GetDobotStatus

KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetDobotStatus",
    "params": {
        "portName": "192.168.5.1"
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
        "alarms": [null, [],
            [],
            [],
            []
        ],
        "armOrientation": 1,
        "autoManual": "manual",
        "cartesianCoordinate": [400, 0, 0, 0],
        "controlMode": "disable",
        "coordinate": "joint",
        "inputs": [0, 0, 0, 0, 0, 0, 0, 0],
        "jogMode": "jog",
        "jointCoordinate": [0, 0, 0, 0],
        "outputs": [0, 0, 0, 0, 0, 0, 0, 0],
        "toolCoordinate": 0,
        "userCoordinate": 0
    }
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com