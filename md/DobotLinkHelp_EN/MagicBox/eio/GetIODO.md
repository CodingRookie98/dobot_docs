# 5.7.4 GetIODO

Read I / O output level



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | EIO 
address（0~25） |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| level | int | yes | output level (0: low level, 1: high 
    level) |
| port | int | yes | EIO address (0 ~ 
25) |



KeyWords:

portName: string

port: int (0~25)

level: int (0~1)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIODO",
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
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "level": 0,        "port": 1    }}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com