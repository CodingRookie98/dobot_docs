# 4.10.5 SetPTPCoordinateParams

Set coordinate axis point parameters

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |
| xyzVelocity | float | yes | xyz 3-axis speed in PTP mode |
| rVelocity | float | yes | terminal speed in PTP mode |
| xyzAcceleration | float | yes | xyz 3-axis acceleration in PTP mode |
| rAcceleration | float | yes | terminal acceleration in PTP mode |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation 
      succeeded, false: operation failed) |






KeyWords:

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetPTPCoordinateParams",
    "params": {
        "portName": "COM4",
        "xyzVelocity": 200,
        "rVelocity": 100,
        "xyzAcceleration": 200,
        "rAcceleration": 100,
        "isQueued": false
    }
}
```

OUTPUT:

```json

{    "id": 1,     "jsonrpc": "2.0",    "result": true}


```json


```

Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com