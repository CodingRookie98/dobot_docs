# 7.25.3 GetHotkey

功能:

快捷键查询接口,用于第六轴末端的按钮控制



INPUT:

```json
{    "id": 1,    "jsonrpc": "2.0",    "method": "dobotlink.CR.GetHotkey",    "params": {        "portName": "192.168.5.1"    }}
```

 OUTPUT： 

```json


```json
{
     "id": 1,
      "jsonrpc": "2.0",

    "result": 
{   "down": [17, 0, 18, 1],  "downApi": "DO1_OFF_DO2_ON",  "id": 3,  "mode": 0,  "name": "Terminal-IO",  "up": [17, 0, 18, 0],  "upApi": "DO1_OFF_DO2_OFF" }}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)