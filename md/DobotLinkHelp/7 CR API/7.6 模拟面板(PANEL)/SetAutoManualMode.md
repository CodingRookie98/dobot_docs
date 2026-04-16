### 7.6.1 SetAutoManualMode

**KeyWords:**

portName: string

data: object

value: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetAutoManualMode",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "value": "auto"/"manual"
        }
    }
}
```
