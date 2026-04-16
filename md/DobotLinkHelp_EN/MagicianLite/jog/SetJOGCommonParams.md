# 4.9.5 SetJOGCommonParams

Set jog common parameters


 request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| velocityRatio | float | yes | speed ratio, joint jogging and axis jogging 
      are shared |
| accelerationRatio | float | yes | acceleration ratio, joint inching and 
      coordinate axis inching are shared |
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

velocityRatio: float

accelerationRatio: float

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetJOGCommonParams",
    "params": {
        "portName": "COM4",
        "velocityRatio": 100,
        "accelerationRatio": 50,
        "isQueued": false
    }
}
```





OUTPUT:

```json

```json
{
    "id": 1,     "jsonrpc": "2.0",    "result": true
}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com