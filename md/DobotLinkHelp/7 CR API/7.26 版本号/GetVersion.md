### 7.26.1 GetVersion

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetVersion",
    "params": {
        "portName": "192.168.5.1"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "algs": "1.2.22",
        "control": "3.2.3.0",
        "system": "1.0.0",
        "unio": "2.0.0.0",
        "safeio": "2.0.4.0",
        "servo": "2.0.0.0",
        "terminal": "2.0.0.0",
        "feedback": "2.0.2.0"
    }
}
```
