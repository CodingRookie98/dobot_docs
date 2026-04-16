# 9.4.5 SetMoveSpeed

Description: 设置底盘移动速度 

KeyWords:

portName: string

x: float(前进速度)cm/s

y: float(横移速度)cm/s

r: float(旋转速度)deg/s



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetMoveSpeed",
    "params": {
        "portName": "COM4",
        "x": 10.0,
        "y": 10.0,
        "r": 10.0 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)