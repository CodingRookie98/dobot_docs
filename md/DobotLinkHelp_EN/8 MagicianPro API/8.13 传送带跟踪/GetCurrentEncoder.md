**Description: 获取当前编码器值**

**KeyWords:**

portName: string

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetCurrentEncoder",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "conveyor_index": int
        }
    }
}
```