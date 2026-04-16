# 5.7.11 SetColorSensor

Set color sensor

request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | port to use capability |
| enable | bool | yes | use capability (true: yes, false: no) |
| version | int | yes | sensor version to use |
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

port: int (0~25)

enable: bool

version: int

*isQueued: bool (default:false)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetColorSensor",
    "params": {
        "portName": "COM4",
        "port": 1,
        "enable": true,
        "version": 1,
        "isQueued": false
    }
}
```

OUTPUT:

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com