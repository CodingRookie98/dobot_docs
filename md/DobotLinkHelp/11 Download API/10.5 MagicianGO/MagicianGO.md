## 10.5 MagicianGO

**Description: MagicianGO的固件升级接口**

**KeyWords:**

device: string

version: string, 为8位数字版本号，后面补0. 如固件文件版本号是V0.0.0.4,
则version为"00040000"

fileName: string,
固件文件的路径，如果路径为空，则使用link下的默认固件文件.
固件前缀为CarTemp，后缀为.bin

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.StartFirmware",
    "params": {
        "device": "MagicianGO",
        "COM": "COM14",
        "version": "00040000",
        "fileName": "D:/download/CarTempV0.0.0.4.bin"
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

Notification: 通知消息，数字是进度

```json
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"5rn"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"40.1rn"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"100rn"
    }
}
```
