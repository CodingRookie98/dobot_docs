# 4.2.6 GetDeviceTime

Get device system tick clock


request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |

响应参数 result
| field | type | required | explain |
| --- | --- | --- | --- |
| gSystick | string | yes | count value: once every 1ms |
| passtime | string | yes | return a time: the time from the device startup 
      to the present (time format: HH: mm: SS. 
Z) |




KeyWords:

portName: string

gSystick: int

passtime: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetDeviceTime",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "gSystick": 60956409,        "passtime": "16:55:56.409"    }}

```json


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com