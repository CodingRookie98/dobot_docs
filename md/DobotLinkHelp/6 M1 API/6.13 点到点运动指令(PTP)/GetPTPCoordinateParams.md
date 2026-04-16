### 6.13.4 GetPTPCoordinateParams

**KeyWords:**

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetPTPCoordinateParams",
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
        "xyzVelocity": 200,
        "rVelocity": 100,
        "xyzAcceleration": 200,
        "rAcceleration": 100
    }
}
```
