功能:

    全局变量的获取

INPUT:

``` language-json
 {
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetGlobalVar",
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

    "result": {globalVar.json文件内容????} 


 }
```