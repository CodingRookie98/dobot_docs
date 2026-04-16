### 7.4.4 GetTeachJoint

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetTeachJoint",
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
        "velocity": [j1, j2, j3, j4, j5, j6],
        "acceleration": [j1, j2, j3, j4, j5, j6]
    }
}
```
