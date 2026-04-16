### 3.10.2 GetJOGJointParams

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetJOGJointParams",
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
        "velocity": [15, 15, 15, 30],
        "acceleration": [50, 50, 50, 50]
    }
}
```
