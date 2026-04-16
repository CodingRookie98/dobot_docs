# 8.14.26 SetFunctionPostureCalc

Description: 逆解算

KeyWords:

portName: string

mode: int, 1逆解，2正解

tool: int 

user: int 

rawData: list 



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetFunctionPostureCalc",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "mode" : 1,
            "tool" : 0,
            "user" : 0,
            "rawData" : [32.504, 21.379, 32.704, -8.006]
        }
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
        "status": "true",
        "value" :[270.337, 172.251, 15.105, 24.497]
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)