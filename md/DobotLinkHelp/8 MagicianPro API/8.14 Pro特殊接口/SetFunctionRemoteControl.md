### 8.14.24 SetFunctionRemoteControl

**Description: 设置当前模式**

**KeyWords:**

portName: string

mode: string, 模式

name: string, 名字

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetFunctionRemoteControl",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "mode" : "tp",
            "name" : ""
        }
    }
}
```
