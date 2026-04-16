# 9.4.7 SetRotate

Description: 设置底盘旋转角度和旋转角速度，根据角度，速度做自转运动 

KeyWords:

portName: string

r: float(旋转角度）deg

Vr: float(旋转速度）deg/s



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetRotate",
    "params": {
        "portName": "COM4",
        "r": 100.0 ,
        "Vr": 10.0 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)