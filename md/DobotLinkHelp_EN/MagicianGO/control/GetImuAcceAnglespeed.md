# 9.4.25 GetImuSpeed

Description: 获取IMU加速度值与角速度值

KeyWords:

portName: string

ax: float(加速度，g)

ay: float(加速度，g)

az: float(加速度，g)

gx: float(角速度，°/s)

gy: float(角速度，°/s)

gz: float(角速度，°/s)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetImuSpeed",
    "params": {
        "portName": "COM4" 
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
              "ax": 10.0,
	     "ay": 10.0,
	     "az": 10.0,
	     "gx": 10.0,
	     "gy": 10.0,
	     "gz": 10.0 
     }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)