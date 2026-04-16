# 10.4 Camera

Description: K210摄像头的固件升级接口

KeyWords:

device: string, 末端：CameraArm，小车：CameraCar

COM: string，端口号

fileName: string, 固件文件的路径，如果路径为空，则使用link下的默认固件文件. 末端固件前缀为AicamEndstop，小车固件前缀为AicamArm，后缀为.kfpkg

fileName格式: 文件名_版本号_烧录文件数量，进度条的数量为烧录文件数量+1



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.StartFirmware",
    "params": {
        "device": "CameraArm",
        "COM": "COM14",
        "fileName": "D:/download/AicamEndstop_V0.6.2.75_6.kfpkg"
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
        "message":"\rDownloading ISP: |---------------------------------------------| 1.5% \r"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"\rDownloading ISP: |============================-----------------| 63.1% 9kiB/s\r"
    }
} ...
{
    "method": "dobotLink.download.process",
    "jsonrpc": "2.0",
    "params": {
        "message":"\rDownloading ISP: |=============================================| 100.0% 9kiB/s\r\r\n\u001b[32m\u001b[1m[INFO]\u001b[0m Booting From 0x80000000 \u001b[0m\r\n\u001b[32m\u001b[1m[INFO]\u001b[0m Wait For 0.1 second for ISP to Boot \u001b[0m\r\n"
    }
}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com