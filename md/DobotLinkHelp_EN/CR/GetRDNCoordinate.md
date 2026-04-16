# 7.3.30 GetRDNCoordinate

功能: 

 获取exchange接口中的 rdnCoordinate字段



INPUT:

```json
{    "id": 1,    "jsonrpc": "2.0",    "method": "dobotlink.CR.GetRDNCoordinate",    "params": {        "portName": "192.168.5.1"    }}
```

















 OUTPUT： 

```json
{
    "id": 1,
    "jsonrpc": "2.0",    "result": 1/0  // 1 发生碰撞/0 未发生碰撞(普通的碰撞)  }
```


Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)