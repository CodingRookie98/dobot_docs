### 7.4.5 SetTeachCoordinate

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetTeachCoordinate",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "velocity": [x, y, z, a, b, c],
            "acceleration": [x, y, z, a, b, c]
        }
    }
}
```
