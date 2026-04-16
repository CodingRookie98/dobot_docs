# 7.17.3 GetDebugReTrace

功能: 轨迹复现获取



 KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetDebugReTrace",
    "params": {
        "portName": "192.168.5.1"
    }
}
```



OUTPUT:

```json


```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "currentTimes" : xx   //复现次数 
        "isDone":"true/false" //复现完成
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com