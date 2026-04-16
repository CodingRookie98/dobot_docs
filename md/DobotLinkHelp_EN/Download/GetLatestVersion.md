# 10.9 GetLatestVersion

Description: 获取link内最新固件的版本号，如果是lite和box，还有length和md5的信息。摄像头有固件数量cameraNum。其余设备这两个参数返回为空值

KeyWords:

device: string

version: string, 版本号，

length: string, 长度，lite和box切换固件烧录模式要用 

md5: string, md5，lite和box切换固件烧录模式要用

cameraNum: 摄像头的烧录文件数量



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.GetLatestVersion",
    "params": {
        "device": "MagicBox" 
    }
}
```



OUTPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
              "length":"80C50800",
              "md5":"CA1FA5D13E6E0730A194094020600B8D",
              "version":"2.0.0.6",
              "cameraNum" :0
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com