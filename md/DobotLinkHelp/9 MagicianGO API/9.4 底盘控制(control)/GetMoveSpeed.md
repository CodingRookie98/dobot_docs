### 9.4.6 GetMoveSpeed

**Description: 获取底盘移动速度**

**KeyWords:**

portName: string

x: float(0-100)cm/s

y: float(0-100)cm/s

r: float(0-100)deg/s

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetMoveSpeed",
    "params": {
        "portName": "COM4"
    }
}
```
