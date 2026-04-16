### 8.15.7 AuxGetPlaybackJoint

**Description: 获取扩展轴再现参数**

**KeyWords:**

portName: string

velocity : List<float>

acceleration : List<float>

jerk: List<float>

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxGetPlaybackJoint",
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
        "velocity": [100.0, 100.0, 100.0,100.0],
        "acceleration": [100.0, 100.0, 100.0,100.0],
        "jerk": [100.0, 100.0, 100.0, 100.0]
    }
}
```
