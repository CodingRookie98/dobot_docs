功能:

   获取exchange接口中的 rdnCoordinate字段

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetRDNCoordinate",
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
    "result": 1/0  // 1 发生碰撞/0 未发生碰撞(普通的碰撞)
 }
```
