# 4.8.5 SetEndEffectorSuctionCup

Set suction cup status


request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| enable | bool | yes | control whether it is enabled (true: yes, 
      false: no) |
| on | bool | yes | whether the suction cup is sucked (true: 
      yes, false: no) |
| isQueued | bool | no | Queued instructions (true: instructions are 
      queued for execution, false: interrupt the currently executed task and 
      insert it directly for execution) default: 
false |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, false: 
      operation failed) |






KeyWords:

portName: string

enable: bool

on: bool

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetEndEffectorSuctionCup",
    "params": {
        "portName": "COM4",
        "enable": true,
        "on": true,
        "isQueued": false
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com