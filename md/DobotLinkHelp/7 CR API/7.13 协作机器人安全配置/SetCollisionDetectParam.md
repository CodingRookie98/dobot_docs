### 7.13.6 SetCollisionDetectParam

[安全碰撞设置的万能接口，可以修改添加任意字段]{style="FONT-SIZE: 14px; FONT-FAMILY: "Microsoft YaHei", "Segoe UI", system-ui, Roboto, "Droid Sans", "Helvetica Neue", sans-serif, Tahoma, "Segoe UI Symbol", "Myanmar Text", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"}

[]{style="FONT-SIZE: 14px; FONT-FAMILY: "Microsoft YaHei", "Segoe UI", system-ui, Roboto, "Droid Sans", "Helvetica Neue", sans-serif, Tahoma, "Segoe UI Symbol", "Myanmar Text", 微软雅黑; WHITE-SPACE: pre-wrap; WORD-SPACING: 0px; TEXT-TRANSFORM: none; FLOAT: none; FONT-WEIGHT: 400; COLOR: rgb(23,26,29); FONT-STYLE: normal; TEXT-ALIGN: left; ORPHANS: 2; WIDOWS: 2; DISPLAY: inline !important; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; font-variant-ligatures: normal; font-variant-caps: normal; -webkit-text-stroke-width: 0px; text-decoration-style: initial; text-decoration-color: initial; text-decoration-thickness: initial"}

INPUT:

```json
{
 "id": 0,

 "jsonrpc": "2.0",

 "method": "dobotlink.CR.SetCollisionDetectParam",

 "params": {

  "portName": "192.168.1.6",

   "data": {

 "key": "你要修改的字段名称",

 "value": 任意json数据，可以是值，也可以是 jsonArray, jsonObject
  }
 }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
