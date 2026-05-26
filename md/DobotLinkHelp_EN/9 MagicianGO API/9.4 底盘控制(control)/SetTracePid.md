**Description: 设置摄像头巡线的PID**

**KeyWords:**

portName: string

p: float (巡线p值)

i: float (巡线i值)

d: float (巡线d值)

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetTracePid",
    "params": {
        "portName": "COM4",
        "p": 10.0,
        "i": 10.0,
        "d": 10.0
    }
}
```
