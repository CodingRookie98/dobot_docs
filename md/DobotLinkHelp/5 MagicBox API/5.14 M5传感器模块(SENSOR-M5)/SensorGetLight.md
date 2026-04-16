### 12.1.13 SensorGetLight

**读取光线强度**

请求参数 params

  ----------- --------- ----------- ---------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号(2~3)
  ----------- --------- ----------- ---------------

响应参数 result

  -------- ------- ----------- ------------------
  字段    类型   是否必填   说明
  value   int     是         返回值(0~4096)
  -------- ------- ----------- ------------------

**KeyWords:**

portName: string

port: int (2~3)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetLight",
    "params": {
        "portName": "COM4",
        "port": 3
    }
}
```

OUTPUT：

```json
 {
 "id": 1,

 "jsonrpc": "2.0",
  "result": {
 "value": 1022

 }
}
```
