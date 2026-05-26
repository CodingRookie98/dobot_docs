**KeyWords:**

portName: string

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetPlaybackCoordinate",
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
        "velocity": [xyz, abc],
        "acceleration": [xyz, abc],
        "jerk": [xyz, abc]
    }
}
```
