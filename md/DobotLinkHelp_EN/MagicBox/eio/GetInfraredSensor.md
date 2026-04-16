# 5.7.14 GetInfraredSensor

Acquire infrared sensor



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | port to use 
capability |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| status | int | yes | response results (0: acquisition failed, 
      1: acquisition succeeded) |








KeyWords:

portName: string

port: int (0~25)

status: int (0~1)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetInfraredSensor",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```



OUTPUT:

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "status": 1    }}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com