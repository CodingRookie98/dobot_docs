**KeyWords:**

portName: string

type: int (0:JOG 1:PTP)

value: int (0~100 unit:%)

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetLSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1
    }
}
```
