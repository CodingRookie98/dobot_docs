# 9.4.12 SetCoordClosedLoop

Description: 设置世界坐标系下角度闭环

KeyWords:

portName: string

isEnable: int (是否使能角度闭环)

angle: float (角度，°（-180-180）)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetCoordClosedLoop",
    "params": {
        "portName": "COM4",
        "isEnable": 1 ,
        "angle":10
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)