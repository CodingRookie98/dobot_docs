### 7.9.2 SetMoveCmd

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetMoveCmd",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "x" : double,
            "y":double,
            "z":double,
            "r":double
        }
    }
}
```
