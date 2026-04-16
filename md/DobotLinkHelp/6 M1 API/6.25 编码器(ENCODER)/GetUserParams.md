### 6.25.2 GetUserParams

**KeyWords:**

portName: string

userParams: float[8]

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetUserParams",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "userParams": [0,0,0,0,167425616,167951328,167698112,168004624]
    }
}
```
