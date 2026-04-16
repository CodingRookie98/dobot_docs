### 6.11.1 SetJOGJointParams

**KeyWords:**

portName: string

velocity: array(float)

acceleration: array(float)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetJOGJointParams",
    "params": {
        "portName": "COM4",
        "velocity": [15, 15, 15, 30],
        "acceleration": [50, 50, 50, 50],
        "isQueued": false
    }
}
```
