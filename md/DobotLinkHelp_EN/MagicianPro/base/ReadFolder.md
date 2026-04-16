# 8.2.8 ReadFolder

Description: 返回文件夹的文件名和时间

KeyWords:

portName: string

folderName: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.ReadFolder",
    "params": {
        "portName": "192.168.1.6",
        "folderName": "/xxx/xxx"
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
               "a.lua": "2020-11-18 18:00:24",
               "src0.lua": "2021-03-09 09:51:57"
     }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)