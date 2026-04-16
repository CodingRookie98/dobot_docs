### 7.4.15 SetUserCoordinate

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetUserCoordinate",
    "params": {
        "portName": "192.168.5.1",
        "data": [{
            "enable": true,
            "params": [0, 0, 0, 0, 0, 0]
        }]
    }
}
```
