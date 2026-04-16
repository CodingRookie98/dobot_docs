# 12.1.15 SensorGetPEState

Read photoelectric sensor status



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port （0~5） |
| version | int | yes | photoelectric sensor version 
number(0~1) |





response result



| field | type | required | explain |
| --- | --- | --- | --- |
| value | bool | yes | return value (false: occlusion, true: no 
      occlusion) |










KeyWords:

portName: string

port: int (0~5)

version: int (0~1)

value: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetPEState",
    "params": {
        "portName": "COM4",
        "port": 2,
        "version": 1
    }
}
```

OUTPUT：

```json

```json
 {     "id": 1,     "jsonrpc": "2.0",     "result": {         "value": false     } }
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com