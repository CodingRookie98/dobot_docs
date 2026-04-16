# 4.9.2 GetJOGJointParams

Get joint jog parameters


 request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |






 response result

| field | type | required | explain |
| --- | --- | --- | --- |
| velocity | array(float) | yes | 4-axis joint speed |
| acceleration | array(float) | yes | 4-axis joint acceleration |









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
    "method": "dobotlink.MagicianLite.GetJOGJointParams",
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
        "velocity": [15, 15, 15, 30],
        "acceleration": [50, 50, 50, 50]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com