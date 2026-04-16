### 12.1.4 SensorSetRGBLEDState

**打开/关闭 RGBLED**

请求参数 params

  ----------- --------- ----------- -----------------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（0~5）
  index      int      是         LED索引（0~2）
  on         bool     是         LED状态（false:关闭，true:打开）
  ----------- --------- ----------- -----------------------------------

响应参数 result

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

**KeyWords:**

portName: string

port: int (0~5)

index: int (0~2)

on: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetRGBLEDState",
    "params": {
        "portName": "COM4",
        "port": 2,
        "index": 1,
        "on": true
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
