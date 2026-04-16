### 7.6.2 SetThreeSwitch

**KeyWords:**

portName: string

data: object

value: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetThreeSwitch",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "value": "released"/"pressed"
        }
    }
}
```
