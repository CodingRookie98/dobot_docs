### 3.9.6 GetEndEffectorLaser

**获取激光器使能和开关状态**

**KeyWords:**

portName: string

isEnabled: bool

isOn: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetEndEffectorLaser",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "isEnabled": false,
"isOn":false
 }
}
```
