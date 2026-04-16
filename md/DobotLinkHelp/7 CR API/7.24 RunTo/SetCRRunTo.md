### 7.24.1 SetCRRunTo

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCRRunTo",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "value" : "true/false",
            "x":x,
            "y":y,
            "z":z,
            "a":a,
            "b":b,
            "c":c,
            "r":r,
            "d":d,
            "n":n,
            "mode" : "go"/"move"/"jump" ,
            "cfg":cfg,
            "tool":tool,
            "user":user
        }
    }
}
```
