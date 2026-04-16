# 12.1.32 SetSensorHandModel

Initialize gesture recognition module



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port 
（0~5） |







response result




| field | type | required | explain |
| --- | --- | --- | --- |
| InitState | bool | yes | initialization status (return value is true: 
      success, false: failure) |





KeyWords:

portName: string

port : int，0~5



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetSensorHandModel",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "InitState": false    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com