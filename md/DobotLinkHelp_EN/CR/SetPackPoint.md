# 7.25.7 SetPackPoint

功能:

 设置打包姿态（打包姿态）



INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetPackPoint", 
    "params": {
         "portName": "192.168.5.1",
          "data":{"joint":[83,0,-157,154,-39,0]} 
   } }

```

OUTPUT：

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```


Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)