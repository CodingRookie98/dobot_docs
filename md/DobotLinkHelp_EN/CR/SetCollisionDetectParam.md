# 7.13.6 SetCollisionDetectParam

安全碰撞设置的万能接口，可以修改添加任意字段



INPUT:

```json

```json
{
    "id": 0,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCollisionDetectParam",
    "params": {
        "portName": "192.168.1.6",        "data": {            "key": "你要修改的字段名称",
            "value": 任意json数据，可以是值，也可以是 jsonArray, jsonObject         }    }}
```





OUTPUT:

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```json

```json

```json

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)