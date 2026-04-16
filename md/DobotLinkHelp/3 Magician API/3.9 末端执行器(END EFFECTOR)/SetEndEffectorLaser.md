### 3.9.5 SetEndEffectorLaser

**设置激光器使能和开关状态**

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
 "method": "dobotlink.Magician.SetEndEffectorLaser",
 "params": {
 "portName": "192.168.5.1",
"enable": false,
 "on": false,
 "isQueued": false
 }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
