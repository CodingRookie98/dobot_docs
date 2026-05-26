**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetCRRunTo",
    "params": {
        "portName": "192.168.1.6",
        "data": {
             "value": true/false, false是停止运动，true是开始运动
             "x": 0,
             "y": 0,
             "z": 0,
             "a": 0,
             "b": 0,
             "c": 0,
             "r": -1,
             "d": -1,
             "n": -1,
             "mode" : "go"/"move"/"jump" ,
             "cfg": -1,
             "tool": 0,
             "user": 0
        }
    }
}
```
