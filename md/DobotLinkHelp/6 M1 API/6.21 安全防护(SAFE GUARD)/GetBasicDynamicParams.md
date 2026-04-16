### 6.21.6 GetBasicDynamicParams

**KeyWords:**

portName: string

ZZ1,FS1,FV1,ZZ2,MX2,MY2,IA2,FS2,FV2: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetBasicDynamicParams",
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
        "ZZ1": 1.0,
        "FS1": 1.0,
        "FV1": 1.0,
        "ZZ2": 1.0,
        "MX2": 1.0,
        "MY2": 1.0,
        "IA2": 1.0,
        "FS2": 1.0,
        "FV2": 1.0
    }
}
```
