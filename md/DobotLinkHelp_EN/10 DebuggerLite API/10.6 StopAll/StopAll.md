**Description: 结束所有进程**

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.StopAll",
    "params": {}
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "result": true,
        "detial": [
            {
                "dpid": 1,
                "result": true
            },
            {
                "dpid": 2,
                "result": true
            }
        ]
    }
}
```
