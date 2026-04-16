## 10.2 MagicianLite/MagicBox

**Description: lite和box的固件升级接口**

**KeyWords:**

device: string

fileName:
string，固件文件的路径，如果路径为空，则使用link下的默认固件文件。固件文件前缀是MagicianLite或MagicBox,后缀为.dfu

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.StartFirmware",
    "params": {
        "device": "MagicianLite"/"MagicBox",
        "fileName": "D:/download/MagicianLite-V0.0.0.0_120268_CCD50100_5A8FE1D1A023A34DD059D506B64B2A84.dfu"
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

Notification: 通知消息，数字是进度, 有两个进度条

```json
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"rTarget 00: Upgrading - Erase Phase (0)... Duration: 00:00:01"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"rTarget 00: Upgrading - Erase Phase (19)... Duration: 00:00:05"
    }
} ...
{
    "method": "dobotLink.dfudownload.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"rTarget 00: Upgrading - Erase Phase (100)... Duration: 00:00:17rTarget 00: Upgrading - Download Phase (1)..."
    }
}...//第二个进度条
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":" Duration: 00:00:17rTarget 00: Upgrading - Download Phase (2)..."
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":" Duration: 00:00:42rTarget 00: Upgrading - Download Phase (78)..."
    }
}
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":" Duration: 00:00:49rTarget 00: Upgrading - Download Phase (100)...rnUpgrade successful !rn"
    }
}
```
