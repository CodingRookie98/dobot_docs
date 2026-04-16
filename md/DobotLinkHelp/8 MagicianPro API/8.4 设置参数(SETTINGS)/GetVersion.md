### 8.4.21 GetVersion

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetVersion",
    "params": {
        "portName": "192.168.1.6"
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
        "system": "1.0.0"
    }
}
```
