**Description: 设置里程计数据**

**KeyWords:**

portName: string

x: float(小车X轴偏移坐标)cm

y: float(小车y轴偏移坐标)cm

yaw: float(小车航向角)°

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetSpeedometer",
    "params": {
        "portName": "COM4",
        "x": 10.0,
        "y": 10.0,
        "yaw": 10.0
    }
}
```
