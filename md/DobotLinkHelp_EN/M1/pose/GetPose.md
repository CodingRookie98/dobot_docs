# 6.4.1 GetPose

KeyWords:

portName: string

x: float

y: float

z: float

r: float

jointAngle: array(float)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetPose",
    "params": {
        "portName": "COM4"
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
        "x": 134.01580810546875,
        "y": -5.637601852416992,
        "z": 34.831390380859375,
        "r": -2.4088234901428223,
        "jointAngle": [-2.4088234901428223, 10.456664085388184, 41.771934509277344, 0]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com