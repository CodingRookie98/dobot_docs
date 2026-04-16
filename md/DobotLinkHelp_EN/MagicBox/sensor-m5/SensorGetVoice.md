# 12.1.11 SensorGetVoice

Read sound size



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port 
(2~3) |







response result



| field | type | required | explain |
| --- | --- | --- | --- |
| value | int | yes | return value(0~4095) |






KeyWords:

portName: string

port: int (2~3)

value: int (0~4095)



INPUT:



```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetVoice",
    "params": {
        "portName": "COM4",
        "port": 3
    }
}
```

OUTPUT：

```json

```json

{
    "id": 1,
    "jsonrpc": "2.0",    "result": {        "value": 0    }}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com