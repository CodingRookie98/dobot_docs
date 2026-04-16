# 5.12.1 GetColorObjExist

Get the existing color object





request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port (0~5) |
| color | int | yes | color 
identification（1~7） |





response result




| field | type | required | explain |
| --- | --- | --- | --- |
| status | int | yes | detection status, true detected / false not 
      detected |





KeyWords:

portName: string

port: int (0~5， communication port )

color: int (1~7，color identification)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetColorObjExist",
    "params": {
        "portName": "COM4",
        "port": 0,  
        "color": 1 
    }
}
```



OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "status": 0    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com