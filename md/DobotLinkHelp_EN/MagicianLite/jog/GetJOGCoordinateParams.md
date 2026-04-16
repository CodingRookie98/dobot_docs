# 4.9.4 GetJOGCoordinateParams

Get axis jog parameters

 request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  
device |






response result

| field | type | required | explain |
| --- | --- | --- | --- |
| velocity | array(float) | 是 | 4-axis 
      coordinate (x, y, z, 
r) 
      speed |
| acceleration | array(float) | 是 | 4-axis 
      (x, y, z,r) 
      acceleration |





KeyWords:

portName: string

velocity: array(float)

acceleration: array(float)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetJOGCoordinateParams",
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
        "velocity": [60, 60, 60, 60],
        "acceleration": [60, 60, 60, 60]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com