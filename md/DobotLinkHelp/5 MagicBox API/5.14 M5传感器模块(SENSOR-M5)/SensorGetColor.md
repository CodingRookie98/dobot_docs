### 12.1.21 SensorGetColor

**读取颜色传感器**

注：使用该接口前，需先使用SensorColorInit接口

请求参数 params

  ----------- --------- ----------- ----------------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号(0~5)
  index      int      是         颜色索引 (0:red 1:green 2:blue)
  ----------- --------- ----------- ----------------------------------

响应参数 result

  -------- ------- ----------- ---------
  字段    类型   是否必填   说明
  value   int    是         颜色值
  -------- ------- ----------- ---------

**KeyWords:**

portName: string

port: int (0~5)

index: int (0:red 1:green 2:blue)

value: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetColor",
    "params": {
        "portName": "COM4",
        "port": 2,
        "index": 1
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "value": 6
 }
}
```
