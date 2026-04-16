### 6.21.9 SetSafeStrategy

**KeyWords:**

portName: string

strategy: int (0:5sRestart 1:EXForceRestart)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetSafeStrategy",
    "params": {
        "portName": "COM4",
        "strategy": 0
    }
}
```
