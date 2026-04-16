### 6.15.4 GetIOADC

**KeyWords:**

portName: string

port: int (1~20)

value: int (0~4095)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetIOADC",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```
