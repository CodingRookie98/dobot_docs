# 12.1.7 SensorOledDisplay

OLED display



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port  (0~5) |
| x | int | yes | row(0~2) |
| y | int | yes | column(0~9) |
| text | string | yes | character string |







response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |





KeyWords:

portName: string

port: int (0~5)

x: int (0~2)

y: int (0~9)

text: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorOledDisplay",
    "params": {
        "portName": "COM4",
        "port": 2,
        "x": 1,
        "y": 2,
        "text": "Hello Dobot."
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com