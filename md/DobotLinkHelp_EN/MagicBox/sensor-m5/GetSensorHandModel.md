# 12.1.33 GetSensorHandModel

Get gesture recognition module


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port （0~5） |





response result






























| field | type | required | explain |
| --- | --- | --- | --- |
| data | string | yes | identification value: |









KeyWords:

portName: string

port : int，0~5

data: int 

 // REGISTER 0

 GES_RIGHT_FLAG = BIT(0), GES_LEFT_FLAG = BIT(1), GES_UP_FLAG = BIT(2), GES_DOWN_FLAG = BIT(3), GES_FORWARD_FLAG = BIT(4), GES_BACKWARD_FLAG = BIT(5), GES_CLOCKWISE_FLAG = BIT(6), GES_COUNT_CLOCKWISE_FLAG = BIT(7),

 // REGISTER 1

 GES_WAVE_FLAG = BIT(0), READ_ERR = 0xff,



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetSensorHandModel",
    "params": {
        "portName": "COM4",
        "port": 2 
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "data": 255    }}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com