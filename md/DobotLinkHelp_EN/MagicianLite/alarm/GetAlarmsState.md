# 4.6.1 GetAlarmsState

Get alarm status




reuquest params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |

响应参数 result
| field | type | required | explain |
| --- | --- | --- | --- |
| state | array(int) | yes | this 
      array stores the alarm status of each alarm item (1: alarm status, 0: non 
      alarm status) |








KeyWords:

portName: string

state: array(int)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetAlarmsState",
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
        "state": [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com