功能:

获取exchange接口中的 skinValue 字段

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetSkinValue",
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
    "result":  [0,1,2,3,4,5,6,7,8,9,10,11] //12块电子皮肤的数值
}
```
