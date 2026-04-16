# 12.1.2 SensorSetRGBLEDValue

Set RGBLED



Note: before using this interface, you need to initialize the rgbled interface



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port (0~5) |
| index | int | yes | Led number(0~2) |
| red | int | yes | red threshold(0~255) |
| green | int | yes | green threshold(0~255) |
| blue | int | yes | blue 
threshold(0~255) |







 response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation 
      succeeded, false: operation failed) |









KeyWords:

portName: string

port: int (0~5)

index: int (0~2)

red: int (0~255)

green: int (0~255)

blue: int (0~255)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetRGBLEDVlaue",
    "params": {
        "portName": "COM4",
        "port": 2,
        "index": 1,
        "red": 0,
        "green": 120,
        "blue": 200
    }
}
```



OUTPUT:

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com