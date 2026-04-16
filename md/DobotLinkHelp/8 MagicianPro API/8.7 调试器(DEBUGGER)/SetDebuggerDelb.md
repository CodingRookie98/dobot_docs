### 8.7.9 SetDebuggerDelb

**Description: 移除断点**

**KeyWords:**

portName: string

path: string

line: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetDebuggerDelb",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "path": "/dobot/userdata/project/project/MoveJ/src0.lua",
            "line": 2
        }
    }
}
```
