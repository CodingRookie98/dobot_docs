### 7.13.5 SetSafeParams

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetSafeParams",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "safeconfig": {
                "forceConstr"：forceConstrValue,
                "powerConstr": powerConstrValue,
                "velConstr": velConstrValue,
                "monentumConstr": monentumConstrValue
            }
        }
    }
}
```
