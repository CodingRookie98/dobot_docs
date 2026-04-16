## 2.9 GetPluginList

**KeyWords:**

pluginName: string

version: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.api.GetPluginList"
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "MagicDevicePlugin": "3.1.0(protocal:3.2.2)",
        "ArduinoPlugin": "1.0.0",
        "DownloadPlugin": "1.0.0"
    }
}
```
