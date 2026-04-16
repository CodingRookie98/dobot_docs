## 10.1 Prepare

**Description: 初始化脚本进程**

**KeyWords:**

script: string，base64转码后的代码

*portName: string，可选，使用EDU模块的时候用到

*host: string，可选，使用EDU模块的时候用到

*token: string，可选，使用EDU模块的时候用到

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.Prepare",
    "params": {
        "script": "aW1wb3J0IHRpbWUKCndoaWxlIDE6CiAgICBwcmludCgxMTExKQogICAgdGltZS5zbGVlcCgxKQ",
        "portName": "COM4",
        "host": "http://dev.dobotlab.com",
        "token": "CiAgICBwcmludCgogICAgdGltZ"
    }
}
```
