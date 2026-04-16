## 2.12 GetVersion

**KeyWords:**

version: string

protocol: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.api.GetVersion"
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "main": {
            "version": "5.0.0"
        },
        "plugins": {
            "ArduinoPlugin": "1.0.0",
            "DownloadPlugin": "1.0.0",
            "MagicDevicePlugin": "3.1.0(protocal:3.2.2)",
            "MicrobitPlugin": "x"
    }
    }
}
```
