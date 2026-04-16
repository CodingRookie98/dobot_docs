INPUT:

```json
{ 
 "id": 1, 
 "jsonrpc": "2.0", 
 "method": "dobotlink.CR.SetRetraceParams",
 "params": { 
 "portName": "192.168.1.6",
"data":{
"multi" : 1 //速度倍数
"const": 1 //const=1:匀速复现,0:非匀速复现
"loop":1 //复现次数
}
 }
}
```

OUTPUT：
:::

<div>



</div>

```json
{ 
 "id": 1, 
 "jsonrpc": "2.0",
  "result":{"value":true/false} 
}
```
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
