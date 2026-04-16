# 7.25.19 SetHardwareEnable

功能:

 用于控制器确定是否判断示教器的硬件I/O



INPUT:

```json
{    "id": 1,    "jsonrpc": "2.0",    "method": "dobotlink.CR.SetHardwareEnable",    "params": {        "portName": "192.168.5.1",        "data":{        "enable" : true/false        }     }}
```
OUTPUT：
```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)