# 4.10.10 GetPTPCommonParams

Get public parameters of points

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| velocityRatio | float | yes | PTP mode speed scale, joint and axis modes share |
| accelerationRatio | float | yes | PTP mode acceleration scale, joint and 
      coordinate axis modes 
share |





KeyWords:

portName: string

velocityRatio: float

accelerationRatio: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPTPCommonParams",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT：

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "accelerationRatio": 123,        "velocityRatio": 123    }}
```json


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com