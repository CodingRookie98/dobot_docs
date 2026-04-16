# 7.17.2 SetDebugReTrace

功能: 轨迹复现设置



KeyWords:

portName: string

data: object



 INPUT:

```json


```json

{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetDebugReTrace",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "cmd" : "start/stop",
            "addr":"filename.csv"
            "mode" : "moveJ/moveL",
            "loopTimes"：int
        }
    }
}
```

 OUTPUT：

```json


```json
{       "id": 1,    "jsonrpc": "2.0",
    "result":{"value":true/false}
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com