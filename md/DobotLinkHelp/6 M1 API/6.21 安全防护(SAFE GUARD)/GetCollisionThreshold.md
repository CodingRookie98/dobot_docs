### 6.21.4 GetCollisionThreshold

**KeyWords:**

portName: string

torDiffJ1: float

torDiffJ2: float

torDiffJ3: float

torDiffJ4: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetCollisionThreshold",
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
        "torDiffJ1": 0.0,
        "torDiffJ2": 0.0,
        "torDiffJ3": 0.0,
        "torDiffJ4": 0.0
    }
}
```
