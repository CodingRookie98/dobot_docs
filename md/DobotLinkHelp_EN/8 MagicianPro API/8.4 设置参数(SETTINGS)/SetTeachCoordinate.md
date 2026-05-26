**KeyWords:**

portName: string

data: object

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetTeachCoordinate",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "velocity": [x, y, z, a, b, c],
            "acceleration": [x, y, z, a, b, c]
        }
    }
}
```