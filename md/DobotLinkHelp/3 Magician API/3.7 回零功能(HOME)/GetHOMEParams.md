### 3.7.2 GetHOMEParams

**KeyWords:**

portName: string

x: float

y: float

z: float

r: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetHOMEParams",
    "params": {
        "portName": "COM4",
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "x": 192.88986206054688,
        "y": 23.918956756591797,
        "z": 67.55459594726562,
        "r": 7.06879997253418
    }
}
```
