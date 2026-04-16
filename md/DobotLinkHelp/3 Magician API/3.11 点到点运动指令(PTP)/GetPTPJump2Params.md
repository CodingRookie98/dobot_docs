### 3.11.17 GetPTPJump2Params

**KeyWords:**

portName: string

zLimit: float

startJumpHeight: float

endJumpHeight: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetPTPJump2Params",
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
        "zLimit": 100,
        "startJumpHeight": 20,
        "endJumpHeight": 20
    }
}
```
