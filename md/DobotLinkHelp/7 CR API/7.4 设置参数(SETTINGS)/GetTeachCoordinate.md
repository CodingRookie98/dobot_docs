### 7.4.6 GetTeachCoordinate

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetTeachCoordinate",
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
        "velocity": [x, y, z, a, b, c],
        "acceleration": [x, y, z, a, b, c]
    }
}
```
