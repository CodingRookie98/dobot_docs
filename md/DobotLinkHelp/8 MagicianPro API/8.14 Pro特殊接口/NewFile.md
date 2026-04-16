### 8.2.5 NewFile

**Description: 新建文件**

**KeyWords:**

portName: string

fileName: string

content: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.NewFile",
    "params": {
        "portName": "192.168.1.6",
        "fileName": "/project/settings/newfile.lua",
        "content": "print(123456)"
    }
}
```
