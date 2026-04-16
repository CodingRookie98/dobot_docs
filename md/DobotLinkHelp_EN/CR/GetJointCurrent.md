# 7.3.27 GetJointCurrent

功能: 

 获取exchange接口中的 jointCurrent 字段 



INPUT: 

```json
{    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetJointCurrent",
    "params": {
         "portName": "192.168.5.1"
     }
}

```

OUTPUT：

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": [j1, j2, j3, j4, j5, j6]
} 
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)