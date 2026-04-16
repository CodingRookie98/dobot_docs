# 4.10.3 SetPTPJointParams

Set joint point parameters

request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| velocity | array（float） | yes | 4-axis joint speed in PTP mode |
| acceleration | array（float） | yes | 4-axis joint acceleration in PTP mode |
| isQueued | bool (default:false) | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | 是 | response result (true: operation 
      succeeded, false: operation failed) |








KeyWords:

portName: string

velocity: array(float)

acceleration: array(float)

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetPTPJointParams",
    "params": {
        "portName": "COM4",
        "velocity": [200, 200, 200, 200],
        "acceleration": [200, 200, 200, 200],
        "isQueued": false
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com