### 9.4.1 SetRunningMode

**Description: 设置运行模式**

**KeyWords:**

portName: string

runningState: int (0:NORMAL MODE 1:SAFE MODE)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetRunningMode",
    "params": {
        "portName": "COM4",
        "runningMode": 1
    }
}
```
