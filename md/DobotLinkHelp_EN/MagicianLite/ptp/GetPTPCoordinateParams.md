# 4.10.6 GetPTPCoordinateParams

Set coordinate axis point parameters

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |




reponse result

| field | type | required | explain |
| --- | --- | --- | --- |
| xyzVelocity | float | yes | xyz 3-axis speed in PTP mode |
| rVelocity | float | yes | terminal speed in PTP mode |
| xyzAcceleration | float | yes | xyz 3-axis acceleration in PTP mode |
| rAcceleration | float | yes | terminal acceleration in PTP 
mode |





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
    "method": "dobotlink.MagicianLite.GetPTPCoordinateParams",
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
        "rVelocity": 100,
        "xyzAcceleration": 200,
        "rAcceleration": 100
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com