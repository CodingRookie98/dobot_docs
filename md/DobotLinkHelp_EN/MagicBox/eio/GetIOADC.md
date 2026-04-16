# 5.7.8 GetIOADC

Read I / O analog-to-digital conversion value


request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | EIO address 
(0~25) |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| port | int | yes | EIO address (0~25) |
| value | int | yes | input ADC 
value(0~4095) |





KeyWords:

portName: string

port: int (0~25)

value: int (0~4095)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOADC",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```



OUTPUT：
```json


```json

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "port": 1,        "value": 0    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com