# 7.25.13 SetApiUpdate

功能: 

 通知控制器更新Dobot+的api 





INPUT:

```json
{    "id": 1,    "jsonrpc": "2.0",    "method": "dobotlink.CR.SetApiUpdate",    "params": {        "portName": "192.168.5.1",        "data":{"path":"/dobot/userdata/project/settings/api.lua"}    }}
```

OUTPUT：

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {"status":true}
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)