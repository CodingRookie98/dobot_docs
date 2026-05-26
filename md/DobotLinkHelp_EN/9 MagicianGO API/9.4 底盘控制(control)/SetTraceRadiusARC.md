**Description: 设置半径圆弧轨迹功能，根据转动半径，角度做圆弧运动**

**KeyWords:**

portName: string

velocity: float（走圆弧轨迹的速度，单位
°/s（度/秒），正值表示逆时针旋转，负值表示顺时针旋转 ）

radius: float（圆弧轨迹半径）(cm)

angle: float（小车绕圆弧转动角度）(deg/s)

mode: int(选择绕圆弧轨迹行走的模式，取值\[1, 2\]，
1-切向运动，2-刷锅运动)

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetArcRad",
    "params": {
        "portName": "COM4",
        "velocity": 10.0,
        "radius": 10.0,
        "angle": 10.0,
        "mode": 1
    }
}
```
