### 8.8.2 SetEmergencyStop

**Description: 设置急停状态**

**KeyWords:**

portName: string

data: object

value: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetEmergencyStop",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "value": true/false
        }
    }
}
```
