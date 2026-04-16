### 9.4.3 SetMoveSpeedTime

**Description: 设置底盘移动速度带时间参数，遥控场景下使用**

**KeyWords:**

portName: string

time: float(time时间后速度清零)s

x: float(前进速度)cm/s

y: float(横移速度)cm/s

r: float(旋转速度)deg/s

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetMoveSpeedTime",
    "params": {
        "portName": "COM4",
        "time": 5.0
        "x": 10.0,
        "y": 10.0,
        "r": 10.0
    }
}
```
