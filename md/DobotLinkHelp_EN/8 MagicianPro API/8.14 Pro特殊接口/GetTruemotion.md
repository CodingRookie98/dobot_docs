**Description: 获取Truemotion功能**

**KeyWords:**

portName: string

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetTruemotion",
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
        "UsingTrueMotion": true,
        "DynamicOptimal": false,
        "UsingAccType": 0,
        "TorqueFeedforward": false,
        "InputECP": false,
        "InputShapingFreq": 5.4348,
        "InputShapingDamp": 0.1238
    }
}
```
