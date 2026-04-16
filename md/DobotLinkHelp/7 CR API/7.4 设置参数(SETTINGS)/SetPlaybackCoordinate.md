### 7.4.9 SetPlaybackCoordinate

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetPlaybackCoordinate",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "velocity": [xyz, abc],
            "acceleration": [xyz, abc],
            "jerk": [xyz, abc]
        }
    }
}
```
