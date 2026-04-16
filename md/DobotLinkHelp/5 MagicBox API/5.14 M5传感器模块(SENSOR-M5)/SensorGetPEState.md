### 12.1.15 SensorGetPEState

**读取光电传感器状态**

请求参数 params

  ----------- --------- ----------- --------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（0~5）
  version    int      是         光电传感器版本号 (0~1)
  ----------- --------- ----------- --------------------------

响应参数 result

  -------- ------- ----------- ------------------------------------
  字段    类型   是否必填   说明
  value   bool    是         返回值(false:有遮挡，true:无遮挡)
  -------- ------- ----------- ------------------------------------

**KeyWords:**

portName: string

port: int (0~5)

version: int (0~1)

value: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetPEState",
    "params": {
        "portName": "COM4",
        "port": 2,
        "version": 1
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "value": false
 }
}
```
