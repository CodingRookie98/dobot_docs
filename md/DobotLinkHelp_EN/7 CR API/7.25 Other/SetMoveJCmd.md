功能:

 设置运动到打包姿态与初始姿态

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetMoveJCmd",
    "params": {
        "portName": "192.168.5.1",
  "data":{
   "value":true, // bool 量 可以为 true 或者false  ，true 为开始运动，false 为停止运动，停止运动可以不带下面的参数
   "joint":[
    0.1,      // 关节坐标值，类型为json 的number 类型
    0.1,
    0.1,

    0.1,

    0.1,

    0.1

    ]

    }

}

}
```

OUTPUT：

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0",

    "result": ???
}
```
