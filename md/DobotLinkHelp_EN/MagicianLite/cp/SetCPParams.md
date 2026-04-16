# 4.13.1 SetCPParams

Set continuous track motion parameters


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| targetAcc | float | yes | m |
| junctionVel | float | yes | m |
| isRealTimeTrack | bool | yes | whether to enable real-time mode (true: Yes, false: no) |
| acc | float | no | m |
| period | float | no | i |
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

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float(isRealTimeTrack = false)

*period: float(isRealTimeTrack = true)

*isQueued: bool (default:false)



INPUT:

```json

```json

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCPParams",
    "params": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100,
        "isQueued": false
    }
}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetCPParams",
    "params": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": true,
        "period": 20,
        "isQueued": false
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",     "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com