### 8.2.11 CopyFolder

**Description: 复制文件夹**

**KeyWords:**

portName: string

url: string（路径）

folderName: string（原来的文件名）

newfolderName: string（复制后的文件名）

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.CopyFolder",
    "params": {
        "portName": "192.168.1.6",
        "url": "/project/***/***"
        "folderName": "test1",
        "newfolderName": "test2"
    }
}
```
