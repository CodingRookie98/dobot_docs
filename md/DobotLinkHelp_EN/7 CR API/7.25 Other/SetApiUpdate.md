功能:

    通知控制器更新Dobot+的api

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetApiUpdate",
    "params": {
        "portName": "192.168.5.1",
        "data":{"path":"/dobot/userdata/project/settings/api.lua"}
    }
}
```

OUTPUT：

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0",

    "result": {"status":true}

}
```