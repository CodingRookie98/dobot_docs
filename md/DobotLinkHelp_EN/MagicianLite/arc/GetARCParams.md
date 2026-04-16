# 4.14.2 GetARCParams

Get arc interpolation function parameters



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |




response result



| field | type | required | explain |
| --- | --- | --- | --- |
| xyzVelocity | float | yes | circular motion XYZ triaxial velocity |
| rVelocity | float | yes | end rotation speed of circular motion |
| xyzAcceleration | float | yes | circular motion XYZ triaxial acceleration |
| rAcceleration | float | yes | rotation acceleration at the end of circular 
      motion |





KeyWords:

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetARCParams",
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
        "xyzVelocity": 200,
        "rVelocity": 200,
        "xyzAcceleration": 200,
        "rAcceleration": 200
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com