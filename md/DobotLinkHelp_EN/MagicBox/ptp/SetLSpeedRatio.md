# 5.6.2 SetLSpeedRatio

Set rail speed ratio

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| type | int | yes | speed 
      parameter type (0: jog, 1: PTP) |
| value | int | yes | speed proportional value (0 ~ 100 unit:%) |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
      false |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |








KeyWords:

portName: string

value: int 0~100(%)

type: int speed parameter type 0:JOG,1:PTP 



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetLSpeedRatio",
    "params": {
        "portName": "COM4",
        "value": 50,
        "type": 0 
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)