### 7.3.6 SetIRControlMode(已废弃)

**KeyWords:**

portName: string

data: object

controlMode: string ('disable', 'enable', 'drag')

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetIRControlMode",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "controlMode": "disable"/"enable"/"drag"
        }
    }
}
```
