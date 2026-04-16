INPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "method": "dobotlink.CR.SetGlobalVar",
 "params": {
 "portName": "192.168.5.1",
"data":{
"var1": {
"globalHold": true, --是否全局保持
"value": 20 --int类型
},
"var2": {
"globalHold": false, --是否全局保持
"value": 20.5 --double型
},
"var3": {
"globalHold": true, --是否全局保持
"value": "string" --string型
},
"var4": {
"globalHold": true, --是否全局保持
"value": true --bool型
},
"var5": {
"globalHold": true, --是否全局保持
"value":{ --point示教点
"armOrientation": [
-1,
-1,
-1,
0
],
"coordinate": [
1,
2,
3,
4,
5,
6
],

"tool": 0,

"user": 0

}

 }

  }

 }

}
```
OUTPUT：

```json
{

 "id": 1,

 "jsonrpc": "2.0",
 "result": {"status":true/false}
}
```
