**Description: 设置增量位置角度闭环**

**KeyWords:**

portName: string

x: float(位移增量, cm)

y: float(位移增量, cm)

angle: float(位移增量, °（-180-180）)

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetIncrementClosedLoop",
    "params": {
        "portName": "COM4" ,
        "x": 10.0,
        "y": 10.0,
        "angle": 10.0
    }
}
```
