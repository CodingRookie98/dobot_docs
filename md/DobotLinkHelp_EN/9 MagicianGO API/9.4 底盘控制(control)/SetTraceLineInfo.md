**Description: 用于Box发送摄像头循迹信息给主板**

**KeyWords:**

portName: string

lineInfo: int

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetTraceLineInfo",
    "params": {
        "portName": "COM4",
        "lineInfo": 1
    }
}
```
