# 5.7.2 GetIOMultiplexing

Get IO multiplexing



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | EIO 
address（0~25） |




response result



| field | type | required | explain |
| --- | --- | --- | --- |
| multiplex | int | yes | reuse function：（ |
| port | int | yes | EIO address（0~25） |



KeyWords:

portName: string

port: int (0~25)

multiplex: int (0~6)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOMultiplexing",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```



OUTPUT:

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "multiplex": 1,        "port": 1    }}

```json


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com