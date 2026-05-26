**Description: 输入文本到脚本进程**

**KeyWords:**

dpid: int，脚本进程内部ID，控制脚本进程唯一标识

cmd: string, 要传给脚本进程的经过base64转码的文本

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.Input",
    "params": {
        "dpid": 1,
        "cmd"： "xxx"
    }
}
```
