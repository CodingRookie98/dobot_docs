**Description: 扩展轴点动**

**KeyWords:**

portName: string

posBtns: List\<bool\>

negBtns: List\<bool\>

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxSetJogCmd",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "posBtns": [true, flase, flase, flase, flase, flase],
            "negBtns": [false, flase, flase, flase, flase, flase]
        }
    }
}
```
