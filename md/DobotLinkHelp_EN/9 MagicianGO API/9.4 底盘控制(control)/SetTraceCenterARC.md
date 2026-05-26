**Description: 设置圆心圆弧轨迹功能，根据转动中心做圆弧运动**

**KeyWords:**

portName: string

velocity: float(deg/s)

x: float(cm)

y: float(cm)

angle: float(deg)

mode: int(1:keep 2:whirling)

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetArcCent",
    "params": {
        "portName": "COM4",
        "velocity": 10.0,
        "x": 10.0,
        "y": 10.0,
        "angle": 10.0,
        "mode": 1
    }
}
```
