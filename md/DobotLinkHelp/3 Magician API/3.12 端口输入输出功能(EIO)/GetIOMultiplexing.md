### 3.12.2 GetIOMultiplexing

**KeyWords:**

portName: string

port: int (0~25)

multiplex: int (0~6)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetIOMultiplexing",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```
