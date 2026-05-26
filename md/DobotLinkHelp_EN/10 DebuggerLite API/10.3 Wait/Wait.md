**Description: 等待脚本进程结束**

**KeyWords:**

dpid: int，脚本进程内部ID，控制脚本进程唯一标识

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Debuggerlite.Wait",
    "params": {
        "dpid": 1
    }
}
```