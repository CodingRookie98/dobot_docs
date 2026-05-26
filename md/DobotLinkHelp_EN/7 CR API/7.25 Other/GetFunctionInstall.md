功能:

    获取当前安装状态

INPUT:

``` language-json

{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetFunctionInstall",
    "params": {
        "portName": "192.168.5.1"
    }
}
```

OUTPUT：

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
  "SlopeAngle":0.0,
  "RotationAngle":0.0
 }
}
```
