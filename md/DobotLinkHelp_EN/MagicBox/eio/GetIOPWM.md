# 5.7.6 GetIOPWM

Get I / O PWM output



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | EIO 
address（0~25） |





response result




| field | type | required | explain |
| --- | --- | --- | --- |
| dutyCycle | float | yes | PWM  duty cycle 0~100 |
| frequency | float | yes | PWM frequency (10Hz~1MHz) |
| port | int | yes | EIO 
address（0~25） |





KeyWords:

portName: string

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOPWM",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```



OUTPUT:
```json


```json



{    "id": 1,    "jsonrpc": "2.0",       "result": {        "dutyCycle": 30,        "frequency": 10.199999809265137,        "port": 1    }}
```

Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com