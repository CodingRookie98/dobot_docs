# 8.14.9 GetCollisionDetect

Description: 获取安全碰撞参数

KeyWords:

portName: string

data: object

value: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetCollisionDetect",
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
      
         "Level": 2,
         "Level1": [
            30,
            30,
            30,
            10,
            10,
            10
         ],
        "Level2": [
            25,
            25,
            25,
            8,
            8,
            8
         ],
        "Level3": [
            20,
            20,
            20,
            6,
            6,
            6
        ],
        "Level4": [
            15,
            15,
            15,
            4,
            4,
            4
        ],
        "Level5": [
            10,
            10,
            10,
            3,
            3,
            3
        ],
       "mode": 0,
       "value": false
 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)