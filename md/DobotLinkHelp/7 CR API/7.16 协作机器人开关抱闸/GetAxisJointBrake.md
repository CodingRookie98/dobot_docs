### 7.16.2 GetAxisJointBrake

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetAxisJointBrake",
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
        "joint1": true/false,
        "joint2": true/false,
        "joint3": true/false,
        "joint4": true/false,
        "joint5": true/false,
        "joint6": true/false
    }
}
```
