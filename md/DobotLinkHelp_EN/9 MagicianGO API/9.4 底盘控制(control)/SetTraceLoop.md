**Description: Set trace loop enable (control whether the chassis performs line patrol PID calculation)**

**KeyWords:**

portName: string

enable: bool

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetTraceLoop",
    "params": {
        "portName": "COM4",
        "enable": true
    }
}
```
