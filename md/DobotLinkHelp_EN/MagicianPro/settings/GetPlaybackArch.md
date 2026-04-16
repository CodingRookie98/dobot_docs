# 8.4.14 GetPlaybackArch

KeyWords:

portName: string

data: object



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetPlaybackArch",
    "params": {
        "portName": "192.168.1.6"
    }
}
```



OUTPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result":  [{
            "enable": true,
            "params": {
                "startHeight": 10,
                "endHeight": 15,
                "zLimit": 200
            }
        }, {
            "enable": false,
            "params": {
                "startHeight": 11,
                "endHeight": 20,
                "zLimit": 200
            }
    }]
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)