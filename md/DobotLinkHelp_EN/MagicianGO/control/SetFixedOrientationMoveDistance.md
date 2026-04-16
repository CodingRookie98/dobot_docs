# 9.4.8 SetMoveDist

Description: 设置底盘X轴Y轴移动速度和距离，根据距离，速度移动

KeyWords:

portName: string

x: float(前进距离)cm

y: float(横移距离)cm

Vx: float(前进速度)cm/s

Vx: float(横移速度)cm/s



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetMoveDist",
    "params": {
        "portName": "COM4",
        "x": 10.0,
        "y": 10.0,
        "Vx": 10.0,
        "Vy": 10.0 
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)