**KeyWords:**

portName: string

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetTeachJoint",
    "params": {
        "portName": "192.168.5.1"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "velocity": [j1, j2, j3, j4, j5, j6],
        "acceleration": [j1, j2, j3, j4, j5, j6]
    }
}
```
