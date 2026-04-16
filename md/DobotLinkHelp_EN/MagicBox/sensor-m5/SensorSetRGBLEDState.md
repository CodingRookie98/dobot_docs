# 12.1.4 SensorSetRGBLEDState

Open/Close RGBLED



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port  （0~5） |
| index | int | yes | LED index （0~2） |
| on | bool | yes | LED 
status（false:close，true:open） |





response result

| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |








KeyWords:

portName: string

port: int (0~5)

index: int (0~2)

on: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetRGBLEDState",
    "params": {
        "portName": "COM4",
        "port": 2,
        "index": 1,
        "on": true
    }
}
```

OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com