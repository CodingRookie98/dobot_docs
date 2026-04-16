# 12.1.25 SensorXBeeReceive

XBee receive



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port 
(2) |





 response result




| field | type | required | explain |
| --- | --- | --- | --- |
| text | string | yes | receive string |









KeyWords:

portName: string

port: int (2)

text: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorXBeeReceive",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "text": ""    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com