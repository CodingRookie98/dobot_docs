### 3.11.6 SetPTPJointParams

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
    "method": "dobotlink.Magician.SetPTPJointParams",
    "params": {
        "portName": "COM4",
        "velocity": [200, 200, 200, 200],
        "acceleration": [200, 200, 200, 200],
        "isQueued": false
    }
}
```
