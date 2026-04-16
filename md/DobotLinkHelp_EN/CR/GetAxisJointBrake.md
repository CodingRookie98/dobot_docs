# 7.16.2 GetAxisJointBrake

KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetAxisJointBrake",
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
        "joint1": true/false,
        "joint2": true/false,
        "joint3": true/false,
        "joint4": true/false,
        "joint5": true/false,
        "joint6": true/false
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com