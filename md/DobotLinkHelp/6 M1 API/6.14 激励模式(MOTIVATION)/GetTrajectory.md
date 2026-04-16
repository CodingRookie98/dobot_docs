### 6.14.5 GetTrajectory

**KeyWords:**

portName: string

countMax: int

index: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetTrajectory",
    "params": {
        "portName": "COM4",
        "countMax": 6,
        "index": 2
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "data": [{
            "data1": -2.365460091098452e-27,
            "data2": 2.3341894984448154e-26,
            "data3": 3.525147853802959e+21,
            "data4": 50523042480128
        }, {
            "data1": -4411573802660528000,
            "data2": 71.89108276367188,
            "data3": 0.003694072598591447,
            "data4": 15.23687744140625
        }]
    }
}
```
