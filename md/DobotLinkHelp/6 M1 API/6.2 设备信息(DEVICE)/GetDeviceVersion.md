### 6.2.5 GetDeviceVersion

**KeyWords:**

portName: string

type: int

majorVersion: int

minorVersion: int

revision: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetDeviceVersion",
    "params": {
        "portName": "COM4",
        "type": 2
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "type": 2,
        "majorVersion": 3,
        "minorVersion": 6,
        "revision": 14
    }
}
```
