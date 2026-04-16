### 9.3.5 GetDeviceFwHardwareVersion

**Description: 获取设备硬件版本号**

**KeyWords:**

portName: string

previousVersion: int

reVersion: int

minorVersion: int

majorVersion: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetDeviceFwHardwareVersion",
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
    "result":  {
        "previousVersion": 1,
        "reVersion": 1,
        "minorVersion": 1,
        "majorVersion": 1,
     }
}
```
