### 6.13.6 GetPTPJumpParams

**KeyWords:**

portName: string

isUsingZLimit: true

zLimit: float

jumpHeight: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetPTPJumpParams",
    "params": {
        "portName": "COM4",
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "isUsingZLimit": true,
        "zLimit": 100,
        "jumpHeight": 20
    }
}
```
