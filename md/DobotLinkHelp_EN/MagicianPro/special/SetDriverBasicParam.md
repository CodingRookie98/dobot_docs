# 8.14.5 SetDriverBasicParam

Description: 伺服参数配置

KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetDriverBasicParam",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "index":1~4,//1=0g, 2=250g, 3=500g, 4=750g
        }
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)