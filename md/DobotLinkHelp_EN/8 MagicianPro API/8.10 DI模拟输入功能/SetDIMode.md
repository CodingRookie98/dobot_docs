**Description: 设置DI模式**

**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetDIMode",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "index": 10,
            "mode": 0 //0表示现实模式，1表示模拟模式
        }
    }
}
```
