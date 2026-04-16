### 8.14.3 SetLoadParams

**Description: 设置负载参数**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetLoadParams",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "inertiaX": 0.0,
             "inertiaY": 0.0,
             "inertiaZ": 0.0,
             "loadValue": 0.0
        }
    }
}
```
