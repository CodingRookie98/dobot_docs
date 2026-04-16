### 6.11.4 GetJOGCoordinateParams

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetJOGCoordinateParams",
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
        "velocity": [60, 60, 60, 60],
        "acceleration": [60, 60, 60, 60]
    }
}
```
