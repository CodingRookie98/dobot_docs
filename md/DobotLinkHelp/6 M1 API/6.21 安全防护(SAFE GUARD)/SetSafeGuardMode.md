### 6.21.11 SetSafeGuardMode

**KeyWords:**

portName: string

mode: int (0:SafeGuarDisable 1:SafeGuarImmediate 2:SafeGuarIoTrigger)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetSafeGuardMode",
    "params": {
        "portName": "COM4",
        "mode": 1
    }
}
```
