### 8.4.12 GetPlaybackCoordinate

**KeyWords:**

portName: string

INPUT:

```json
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

```json
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
