### 12.1.14 SensorPEInit

**初始化光电传感器模块**

请求参数 params

  ----------- --------- ----------- --------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（0~5）
  version    int      是         光电传感器版本号 (0~1)
  ----------- --------- ----------- --------------------------

响应参数 result

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

**KeyWords:**

portName: string

port: int (0~5)

version: int (0~1)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorPEInit",
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
 "result": true
}
```
