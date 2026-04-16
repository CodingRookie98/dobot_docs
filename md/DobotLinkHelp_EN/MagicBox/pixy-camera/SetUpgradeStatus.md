# 5.12.2 GetColorObjCoordinate

Get color coordinates



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port (0~5) |
| color | int | yes | color identification(1~7) |
| coordinate | int | yes | coordinate |





response result




| field | type | required | explain |
| --- | --- | --- | --- |
| color | int | yes | color identification |
| coordinate | int | yes | coordinate |





KeyWords:

portName: string

port: int (0~5，端口号)

color: int (1~7，颜色标识)

coordinate: int (1~4, 1代表x,2代表y,3代表l,4代表z)



INPUT:



```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetColorObjCoordinate",
    "params": {
        "portName": "COM4",
        "port": 2,
        "color": 1,
        "coordinate": 1   
    }
}
```



OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "color": 1,        "coordinate": 0    }}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com