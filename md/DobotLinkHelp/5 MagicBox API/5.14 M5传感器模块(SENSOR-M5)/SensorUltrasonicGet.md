### 12.1.17 SensorUltrasonicGet

**读取超声波距离**

请求参数 params

  ----------- --------- ----------- ---------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号(0~5)
  ----------- --------- ----------- ---------------

响应参数 result

  -------- ------- ----------- -------------------
  字段    类型   是否必填   说明
  value   int     是         距离（单位：cm）
  -------- ------- ----------- -------------------

**KeyWords:**

portName: string

port: int (0~5)

value: int (unit: cm)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorUltrasonicGet",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorUltrasonicGet",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```
