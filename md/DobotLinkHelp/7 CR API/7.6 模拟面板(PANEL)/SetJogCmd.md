### 7.6.4 SetJogCmd

**KeyWords:**

portName: string

data: object

posBtns: array(bool) ([x, y, z, a, b, c])

negBtns: array(bool) ([x, y, z, a, b, c])

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetJogCmd",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "posBtns": [true, false, false, false, false, false],
            "negBtns": [false, false, false, false, false, false]
        }
    }
}
```
