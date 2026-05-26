**Description: 获取负载参数**

**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetLoadParams",
    "params": {
        "portName": "192.168.1.6"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
             'inertiaX': 0.0,
             'inertiaY': 0.0,
             'inertiaZ': 0.0,
             'loadValue': 0.0
    }
}
```
