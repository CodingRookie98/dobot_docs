功能:

 协作运动接口,用于获取当前的运动状态

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetSystemTime",
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
        "date" : "2020-11-04",   //日期
        "time" : "16:51:35"    //时间
    }
}
```