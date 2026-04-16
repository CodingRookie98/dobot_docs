# 12.1.27 SensorSYNInit

Initialize speech synthesis module



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port （1） |
| baud | int | yes | baud rate |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |







KeyWords:

portName: string

port: int (1)

baud: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSYNInit",
    "params": {
        "portName": "COM4",
        "port": 1,
        "baud": 9600
    }
}
```



OUTPUT:

```json

```json
{    "id":1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com