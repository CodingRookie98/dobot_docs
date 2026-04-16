### 3.11.7 GetPTPJointParams

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetPTPJointParams",
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
        "velocity": [200, 200, 200, 200],
        "acceleration": [200, 200, 200, 200]
    }
}
```
