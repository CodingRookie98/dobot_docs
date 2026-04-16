# 10.8 GetLatestVersionInfo

Description: 获取最新的固件信息

KeyWords:

device: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.GetLatestVersionInfo",
    "params": {
        "device": "Magician" 
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
             "info": "2020/03/23 Ver2.0.7.0版本  CJT\r\n1，修复GD USB长时间工作挂掉的问题,\r\n2，增加对gd外部flash的支持\r\n3，开启规划算法精度修复的宏\r\n4，修复点动运动触发报警后，点动速度未置0导致发送停止点动指令会运动一段距离的问题\r\n"
   }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com