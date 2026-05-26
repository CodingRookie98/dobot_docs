**Description: 获取K210手动标定的计算结果**

**KeyWords:**

portName: string

april_list: string, 九个图像坐标

device_list: string, 九个机械臂坐标

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetCameraCalibrationData",
    "params": {
        "portName": "COM4",
        "april_list": "[[52.0,27.0],[112.0,27.0],[170.0,27.0],[51.0,59.0],[111.0,58.0],[170.0,59.0],[50.0,93.0],[111.0,92.0],[172.0,92.0]]",
        "device_list": "[[-63.0,-213.1],[1.0,-215.1],[62.5,-217.6],[-64.5,-238.5],[-1.0,-241.2],[60.5,-244.1],[-66.0,-264.9],[-2.5,-267.3],[59.5,-270.5]]"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "data":"max_x_err:0.44,max_y_err:0.6,mean_x_error:0.23,mean_y_error:0.34"
    }
}
```
