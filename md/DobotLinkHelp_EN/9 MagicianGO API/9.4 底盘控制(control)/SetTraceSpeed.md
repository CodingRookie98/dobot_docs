**Description: 用于Box发送摄像头循迹速度给主板**

**KeyWords:**

portName: string

speed: float

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetTraceSpeed",
    "params": {
        "portName": "COM4",
        "speed": 10 
    }
}
```