**Description: 脚本参数获取**

**KeyWords:**

portName: string

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetFunctionScriptParams",
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
            "accelJ": 69.0,
            "accelL": 96.0,
            "archEnd": 9.0,
            "archStart": 8.0,
            "archZLimit": 87.0,
            "speedJ": 47.0,
            "speedL": 74.0
    }
}
```
