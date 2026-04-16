### 9.4.4 SetMoveSpeedDirect

**Description: 设置底盘方向和速度**

**KeyWords:**

portName: string

dir: float(方向，单位：°（-180-180）)

speed: float(移动速度，cm/s)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetMoveSpeedDirect",
    "params": {
        "portName": "COM4",
        "dir": 10.0,
        "speed": 10.0
    }
}
```
