# 12.1.8 SensorKnobInit

Initialize potentiometer



request


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port (2~3) |





 response


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |







KeyWords:

portName: string

port: int (2~3)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorKnobInit",
    "params": {
        "portName": "COM4",
        "port": 3
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com