功能:

 获取打包姿态（打包姿态）

INPUT:

``` language-json
{

     "id": 1,

      "jsonrpc": "2.0",

    "method": "dobotlink.CR.GetPackPoint",
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
    "result": {"joint":[83,0,-157,154,-39,0]}
}
```
