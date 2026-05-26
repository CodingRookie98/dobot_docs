**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetPlaybackCoordinate",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "velocity": [xyz, abc],
            "acceleration": [xyz, abc],
            "jerk": [xyz, abc]
        }
    }
}
```
