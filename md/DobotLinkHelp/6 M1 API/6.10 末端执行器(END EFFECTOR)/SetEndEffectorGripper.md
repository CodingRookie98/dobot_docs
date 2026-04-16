### 6.10.7 SetEndEffectorGripper

**KeyWords:**

portName: string

enable: bool

on: bool

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetEndEffectorGripper",
    "params": {
        "portName": "COM4",
        "enable": true,
        "on": true,
        "isQueued": false
    }
}
```
