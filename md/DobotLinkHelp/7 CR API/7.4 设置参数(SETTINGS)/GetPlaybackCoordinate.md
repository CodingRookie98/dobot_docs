### 7.4.10 GetPlaybackCoordinate

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetPlaybackCoordinate",
    "params": {
        "portName": "192.168.5.1"
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
