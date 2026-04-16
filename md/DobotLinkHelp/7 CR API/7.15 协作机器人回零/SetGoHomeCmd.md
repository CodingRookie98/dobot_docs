### 7.15.1 SetGoHomeCmd

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetGoHomeCmd",
    "params": {
        "portName": "192.168.5.1",
        "data": {
             "value":true/false //true：开始回零，false：停止回零
        }
    }
}
```
