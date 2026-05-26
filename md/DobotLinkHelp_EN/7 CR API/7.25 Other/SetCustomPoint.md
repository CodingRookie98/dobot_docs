功能:

设置初始姿态

INPUT:

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0",

    "method": "dobotlink.CR.SetCustomPoint",

    "params": {
        "portName": "192.168.5.1",
        "data": {"joint":[0.0,0.0,0.0,0.0,0.0,0.0]}
    }

}
```

OUTPUT：

``` language-json

{

      "id": 1,

    "jsonrpc":
"2.0",
    "result": true
}
```
