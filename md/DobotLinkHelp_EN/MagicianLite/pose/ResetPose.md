# 4.5.2 ResetPose

Reset real-time position


request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| manualEnable | bool | yes | reset status (true: reset the manipulator 
      with the angle specified by the user, false: reset automatically) |
| rearArmAngle | int | yes | boom angle |
| frontArmAngle | int | yes | forearm 
angle |




 response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |






KeyWords:

portName: string

manualEnable: bool

*rearArmAngle: float (manualEnable = true)

*frontArmAngle: float (manualEnable = true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.ResetPose",
    "params": {
        "portName": "COM4",
        "manualEnable": true,
        "rearArmAngle": 100,
        "frontArmAngle": 150
    }
}
```

OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com