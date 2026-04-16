# 9.3.5 GetDeviceFwHardwareVersion

Description: 获取设备硬件版本号

KeyWords:

portName: string

previousVersion: int

reVersion: int

minorVersion: int

majorVersion: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetDeviceFwHardwareVersion",
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
    "result":  {
        "previousVersion": 1,
        "reVersion": 1,
        "minorVersion": 1,
        "majorVersion": 1,
     }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)