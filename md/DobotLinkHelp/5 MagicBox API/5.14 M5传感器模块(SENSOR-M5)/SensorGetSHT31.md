### 12.1.19 SensorGetSHT31

**读取温湿度传感器**

请求参数 params

  ----------- --------- ----------- -----------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（0~5）
  ----------- --------- ----------- -----------------

响应参数 result

  ------- ------- ----------- -------
  字段   类型   是否必填   说明
  tem    int    是         温度
  hum    int    是         湿度
  ------- ------- ----------- -------

**KeyWords:**

portName: string

port: int (0~5)

tem: int

hum: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetSHT31",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "hum": 0,
 "tem": 0
 }
}
```
