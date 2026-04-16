# 4.8.6 GetEndEffectorSuctionCup

Get SuctionCup Status

request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |




reponse result

| field | type | required | explain |
| --- | --- | --- | --- |
| isEnabled | bool | yes | control whether it is enabled (true: yes, false: 
      no) |
| isOn | bool | yes | whether the suction cup 
    is sucked（true：yes，false：no） |





KeyWords:

portName: string

isEnabled: bool

isOn: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorSuctionCup",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT：

```json

{    "id": 1,    "jsonrpc": "2.0",
    "result": {        "isEnabled": false,        "isOn": true
      }
 }

```json
 

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com