# 9.4.38 SetCommuTimeout

Description: 设置通讯超时时间，注意！该接口会影响到所有Magician系列的设备

KeyWords:

portName: string

timeout: int (ms )



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetCommuTimeout",
    "params": {
        "portName": "COM4",
        "timeout": 10000 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)