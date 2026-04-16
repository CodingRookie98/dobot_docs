## 10.6 StopAll

**Description: 结束所有进程**

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.StopAll",
    "params": {}
}
```

OUTPUT:

```json
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
