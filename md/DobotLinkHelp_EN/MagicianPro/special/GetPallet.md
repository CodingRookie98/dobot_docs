# 8.14.30 GetPallet

Description: 获取托盘数据

KeyWords:

portName: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetPallet",
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
    "result": {
             [ 
               {
                 "count": {
                        "x": 3,
                        "y": 4,
                        "z": 5
                  },
                 "direction": 0,
                 "distance": {
                        "x": 5,
                        "y": 5,
                        "z": 5
                  },
                 "firstPoint": {
                        "a": 0,
                        "b": 0,
                        "c": 0,
                        "x": 0,
                        "y": 0,
                        "z": 0
                  },
                 "id": 0,
                 "name": "test1",
                 "preparePoint": {
                        "a": 0,
                        "b": 0,
                        "c": 0,
                        "x": 0,
                        "y": 0,
                        "z": 0
                  },
                 "safePoint": {
                        "a": 0,
                        "auto": false,
                        "b": 0,
                        "c": 0,
                        "x": 0,
                        "y": 0,
                        "z": 0
                 },
                 "userCoord": 0
              },
             {
                ...
             }
         ]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)