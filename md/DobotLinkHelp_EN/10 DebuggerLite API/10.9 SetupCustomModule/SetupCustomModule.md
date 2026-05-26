**Description: 安装自定义Python模块**

**KeyWords:**

fileName: int，文件名

fileContext: int，base64转码后的文件内容

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.SetupCustomModule",
    "params": {
        "fileName": "abc.py",
        "fileContext": "xxxxxxxx"
    }
}
```
