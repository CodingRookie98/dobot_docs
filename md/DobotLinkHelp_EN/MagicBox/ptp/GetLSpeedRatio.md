# 5.6.3 GetLSpeedRatio

Get rail speed ratio





request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| type | int | yes | speed parameter type (0: jog, 1: 
      PTP) |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| value | int | yes | speed proportional value (0 ~ 100 unit:%) |
| type | int | yes | speed 
      parameter type (0: jog, 1: 
PTP) |







KeyWords:

portName: string

type: int speed parameter type 0:JOG,1:PTP



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetLSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 0 
    }
}
```



OUTPUT:

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "type": 0,        "value": 50    }}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)