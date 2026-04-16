# 12.1.21 SensorGetColor

Read color sensor



 Note: before using this interface, you need to use the SensorColorInit interface



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port (0~5) |
| index | int | yes | color index (0:red 1:green 
2:blue) |







response result


| field | type | required | explain |
| --- | --- | --- | --- |
| value | int | yes | color 
value |







KeyWords:

portName: string

port: int (0~5)

index: int (0:red 1:green 2:blue)

value: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetColor",
    "params": {
        "portName": "COM4",
        "port": 2,
        "index": 1
    }
}
```



OUTPUT：

```json

```json
{     "id": 1,     "jsonrpc": "2.0",     "result": {         "value": 6     } }
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com