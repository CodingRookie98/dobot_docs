# 4.7.2 GetHOMEParams

Get zero return parameter



reuqest params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |



response result
| field | type | required | explain |
| --- | --- | --- | --- |
| x | float | yes | current x position |
| y | float | yes | current y position |
| z | float | yes | current z position |
| r | float | yes | current r 
location |




KeyWords:

portName: string

x: float

y: float

z: float

r: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetHOMEParams",
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
        "x": 192.88986206054688,
        "y": 23.918956756591797,
        "z": 67.55459594726562,
        "r": 7.06879997253418
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com