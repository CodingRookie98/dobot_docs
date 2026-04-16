# 10.3 Magician

Description:Magician的固件升级接口

KeyWords:

device: string

COM: string，端口号

is3DPrinter: bool，是否3D打印机固件

fileName: string，固件文件的路径，如果路径为空，则使用link下的默认固件文件. 固件前缀为DobotMCU，后缀为.hex



INPUT:

```json

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

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
}
```



 Notification: 通知消息，数字是进度

```json

```json
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"WRITE_MEMORY:stage3-Start writing datas operations...0\r\n"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"WRITE_MEMORY:stage3-Start writing datas operations...99\r\n"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"WRITE_MEMORY:stage4-writing memory datas success!\r\n"
    }
}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com