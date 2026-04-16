# 4.5.3 CheckPoseLimit

Check point limit



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| isJoint | bool | yes | Control mode 
      (true indicates joint coordinate system, x, y, z and r below correspond to 
      j1, j2, j3 and j4, false indicates Cartesian coordinate system, and x y z 
      r is x y z r) |
| x | float | yes | current x position |
| y | float | yes | current y position |
| z | float | yes | current z position |
| r | float | yes | current r 
position |




 response result
| field | type | required | explain |
| --- | --- | --- | --- |
| isLimited | bool | yes | reponse result （True: the operation succeeded, 
      false: the operation failed） |








KeyWords:

portName: string

isJoint: bool (default:false)

x: float

y: float

z: float

r: float

isLimited: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.CheckPoseLimit",
    "params": {
        "portName": "COM4",
        "isJoint": false,
        "x": 100.6,
        "y": 260.0,
        "z": 20.0,
        "r": 0.0
    }
}
```



OUTPUT：

```json
 {     "id": 1,     "jsonrpc": "2.0",     "result": {         "isLimited": false     } }
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com