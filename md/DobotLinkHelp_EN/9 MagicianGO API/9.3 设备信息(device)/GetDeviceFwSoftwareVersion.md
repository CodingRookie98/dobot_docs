**Description: 获取设备软件版本号**

**KeyWords:**

portName: string

previousVersion: int

reVersion: int

minorVersion: int

majorVersion: int

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetDeviceFwSoftwareVersion",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "previousVersion": 1,
        "reVersion": 1,
        "minorVersion": 1,
        "majorVersion": 1,
    }
}
```
