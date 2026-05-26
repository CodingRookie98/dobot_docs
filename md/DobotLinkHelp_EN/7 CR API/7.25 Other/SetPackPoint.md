功能:

 设置打包姿态（打包姿态）

INPUT:

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0",

    "method": "dobotlink.CR.SetPackPoint",

    "params": {

         "portName": "192.168.5.1",

          "data":{"joint":[83,0,-157,154,-39,0]}

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
