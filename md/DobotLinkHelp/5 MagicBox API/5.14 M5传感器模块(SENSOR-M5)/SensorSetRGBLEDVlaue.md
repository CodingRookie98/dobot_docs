### 12.1.2 SensorSetRGBLEDVlaue

**设置RGBLED**

注：使用该接口前，需先使用 初始化RGBLED接口

请求参数 params

  ----------- --------- ----------- -------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号(0~5)
  index      int     是         led编号(0~2)
  red        int      是         红色阈值(0~255)
  green      int      是         绿色阈值(0~255)
  blue       int      是         蓝色阈值(0~255)
  ----------- --------- ----------- -------------------

响应参数 result

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

**KeyWords:**

portName: string

port: int (0~5)

index: int (0~2)

red: int (0~255)

green: int (0~255)

blue: int (0~255)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetRGBLEDVlaue",
    "params": {
        "portName": "COM4",
        "port": 2,
        "index": 1,
        "red": 0,
        "green": 120,
        "blue": 200
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
