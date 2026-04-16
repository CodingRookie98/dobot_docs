# 12.1.17 SensorUltrasonicGet

Read ultrasonic distance


request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port 
(0~5) |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| value | int | yes | distance（unit：cm） |









KeyWords:

portName: string

port: int (0~5)

value: int (unit: cm)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorUltrasonicGet",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorUltrasonicGet",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com