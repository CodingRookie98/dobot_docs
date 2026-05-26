**Description: 获取K210识别标记模块信息**

**KeyWords:**

portName: string

angle: int

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetArmCameraObj",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "count" : 2  //返回多少组数据,暂定最大值为5
    "dl_obj" :[
             {
            "x" : 1, //x坐标
            "y" : 1, //Y坐标
            "w" : 1, //物体W宽度
            "h" : 1, //物体H高度
            "id" : 1 //类型
             },
             {
            "x" : 1, //x坐标
            "y" : 1, //Y坐标
            "w" : 1, //物体W宽度
            "h" : 1, //物体H高度
            "id" : 2 //类型
             }
    ]

    }
}
```
