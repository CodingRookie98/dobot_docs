功能:

    设置当前安装状态  

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetFunctionInstall",
    "params": {
        "portName": "192.168.5.1",
        "data":{
        "SlopeAngle":0.0,
        "RotationAngle":0.0
        }
    }
}
```

OUTPUT：

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
}
```