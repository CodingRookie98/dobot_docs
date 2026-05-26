**Description: 设置底盘旋转角度和旋转角速度，根据角度，速度做自转运动**

**KeyWords:**

portName: string

r: float(旋转角度）deg

Vr: float(旋转速度）deg/s

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetRotate",
    "params": {
        "portName": "COM4",
        "r": 100.0 ,
        "Vr": 10.0
    }
}
```
