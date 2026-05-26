### 9.4.39 SetTraceLoop

**Description: 设置巡线循环使能（控制底盘是否进行巡线PID计算）**

**KeyWords:**

portName: string

enable: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetTraceLoop",
    "params": {
        "portName": "COM4",
        "enable": true
    }
}
```
