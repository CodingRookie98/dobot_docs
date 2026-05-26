**Description: 获取脚本进程状态**

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.GetProcessStatus",
    "params": {}
}
```

 

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": [
        {
            "dpid": 1,
            "isRunning": true
        },
        {
            "dpid": 2,
            "isRunning": false
        }
    ]
}
```