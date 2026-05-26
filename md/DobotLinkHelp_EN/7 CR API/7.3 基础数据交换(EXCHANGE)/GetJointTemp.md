功能:

   获取exchange接口中的 jointTemp 字段

INPUT:

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0",

    "method": "dobotlink.CR.GetJointTemp",

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

    "result": [j1, j2, j3, j4, j5, j6]

}
```
