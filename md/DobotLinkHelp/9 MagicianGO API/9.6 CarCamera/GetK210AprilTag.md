### 9.5.3 GetArmCameraTag

**Description: 获取识别AprilTag标签信息**

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetArmCameraTag",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
      "count" : 2  //返回多少组数据,暂定最大值为5
    "aptag_obj" : [
        {
            "x" : 123, //x坐标
            "y" : 51, //Y坐标
            "w" : 43, //物体W宽度
            "h" : 34, //物体H高度
            "id" : 1, //类型
                  "rot" : 258.2  //旋转角度
        },
        {
            "x" : 156, //x坐标
            "y" : 91, //Y坐标
            "w" : 17, //物体W宽度
            "h" : 71, //物体H高度
            "id" : 2, //类型
                  "rot" : 21.5  //旋转角度
        }
    }
     ]

}
```
