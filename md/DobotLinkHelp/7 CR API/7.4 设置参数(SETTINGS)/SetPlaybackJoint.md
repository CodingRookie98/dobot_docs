### 7.4.7 SetPlaybackJoint

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetPlaybackJoint",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "velocity": [j1, j2, j3, j4, j5, j6],
            "acceleration": [j1, j2, j3, j4, j5, j6],
            "jerk": [j1, j2, j3, j4, j5, j6]
        }
    }
}
```
