### 3.2.5 GetDeviceVersion

**KeyWords:**

portName: string

majorVersion: int

minorVersion: int

revision: int

hwVersion: int

deviceName: 设备名称

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetDeviceVersion",
    "params": {
        "portName": "COM4",
        "deviceName":"Magician"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "majorVersion": 3,
        "minorVersion": 6,
        "revision": 14,
        "hwVersion": 1
    }
}
```
