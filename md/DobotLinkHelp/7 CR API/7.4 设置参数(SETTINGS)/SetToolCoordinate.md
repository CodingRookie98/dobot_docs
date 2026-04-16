### 7.4.13 SetToolCoordinate

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetToolCoordinate",
    "params": {
        "portName": "192.168.5.1",
        "data": [{
            "enable": true,
            "params": [0, 0, 0, 0, 0, 0]
        }]
    }
}
```
