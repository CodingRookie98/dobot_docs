# 7.13.3 SetAdvancedFunc

KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetAdvancedFunc",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "dynamicOptimal":true/false, //开启-关闭力矩约束功能
            "usingAccType":xx,    //1表示7段规划，为0表示5段规划
        }
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com