**KeyWords:**

portName: string

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetTeachCoordinate",
    "params": {
        "portName": "192.168.1.6"
    }
}
```

 

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "velocity": [x, y, z, a, b, c],
        "acceleration": [x, y, z, a, b, c]
    }
}
```