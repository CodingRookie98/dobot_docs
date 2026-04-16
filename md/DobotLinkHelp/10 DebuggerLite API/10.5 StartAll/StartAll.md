## 10.5 StartAll

**Description: 启动所有脚本进程**

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.StartAll",
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
