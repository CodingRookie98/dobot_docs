## 10.3 Magician

**Description:Magician的固件升级接口**

**KeyWords:**

device: string

COM: string，端口号

is3DPrinter: bool，是否3D打印机固件

fileName:
string，固件文件的路径，如果路径为空，则使用link下的默认固件文件.
固件前缀为DobotMCU，后缀为.hex

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.StartFirmware",
    "params": {
        "device": "Magician",
        "COM": "COM14",
        "is3DPrinter": false,
        "fileName": "D:/download/DobotMCU_V3.7.0.1.hex"
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
        "message":"WRITE_MEMORY:stage3-Start writing datas operations...0rn"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"WRITE_MEMORY:stage3-Start writing datas operations...99rn"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"WRITE_MEMORY:stage4-writing memory datas success!rn"
    }
}
```
