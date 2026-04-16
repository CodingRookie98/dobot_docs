# 4.13.2 GetCPParams

Obtain continuous motion trajectory parameters



request params


| field | type | requried | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |






 response result



| field | type | requried | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| targetAcc | float | yes | maximum planned acceleration |
| junctionVel | float | yes | maximum corner acceleration |
| isRealTimeTrack | bool | yes | whether to enable real-time mode (true: yes, false: no) |
| acc | float | no | maximum actual acceleration, used in non real time 
      mode |
| period | float | no | interpolation cycle, used in real-time 
  mode |





KeyWords:

portName: string

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float(isRealTimeTrack = false)

*period: float(isRealTimeTrack = true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetCPParams",
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
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100
    }
}
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "isRealTimeTrack": true,        "junctionVel": 100,        "period": 20,        "targetAcc": 200    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com