# 5.4.2 GetServoAngle

Obtain the angle of the steering gear



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |






 response result
| field | type | required | explain |
| --- | --- | --- | --- |
| angle | int | yes | angle of steering gear (+ / - 180) |
| index | int | yes | steering gear serial 
number |






KeyWords:

portName: string

index: int

angle: float (+/-180)



INPUT:



```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetServoAngle",
    "params": {
        "portName": "COM4",
        "index": 2
    }
}
```

OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "angle": -270,        "index": 2    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com