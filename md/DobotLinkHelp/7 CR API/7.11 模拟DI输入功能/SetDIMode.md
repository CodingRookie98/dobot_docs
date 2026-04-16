### 7.11.1 SetDIMode

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetDIMode",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "index": 10,
            "mode": 0 //0表示现实模式，1表示模拟模式
        }
    }
}
```
