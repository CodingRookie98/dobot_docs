# 12.1.29 SensorSetSYNMusic

Set voice to play music



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port（1） |
| type | int | yes | voice type (0: background tone 1: sound 
      effect 2: prompt tone) |
| index | int | yes | speech 
index |





response result



| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |






KeyWords:

portName: string

port: int (1)

type: int(0: background tone 1: sound effect 2: prompt tone)

index: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetSYNMusic",
    "params": {
        "portName": "COM4",
        "port": 1,
        "type": 0,
        "index": 2
    }
}
```



OUTPUT：

```json

```json


{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com