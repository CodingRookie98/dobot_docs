功能:

     轨迹复现高级设置

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetRetraceParams",
    "params": {
        "portName": "192.168.1.6",
        "data":{
           "multi" : 1          //速度倍数
           "const": 1          //const=1:匀速复现,0:非匀速复现
           "loop":1           //复现次数
          }
    }
}
```

OUTPUT：

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
     "result":{"value":true/false}
}
```
