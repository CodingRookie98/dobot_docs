功能:

    用于控制器确定是否判断示教器的硬件I/O

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetHardwareEnable",
    "params": {
        "portName": "192.168.5.1",
        "data":{
        "enable" : true/false
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
