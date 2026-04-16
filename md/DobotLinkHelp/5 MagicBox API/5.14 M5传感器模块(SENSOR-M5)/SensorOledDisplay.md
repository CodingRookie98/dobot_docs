### 12.1.7 SensorOledDisplay

**OLED显示**

请求参数 params

  ----------- --------- ------------ ----------------
  字段      类型    是否必填   说明
  portName   string   是          通信端口
  port       int      是          端口号 (0~5)
  x          int      是          行(0~2)
  y         int      是          列(0~9)
  text       string   是          字符串
  ----------- --------- ------------ ----------------

响应参数 result

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

**KeyWords:**

portName: string

port: int (0~5)

x: int (0~2)

y: int (0~9)

text: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorOledDisplay",
    "params": {
        "portName": "COM4",
        "port": 2,
        "x": 1,
        "y": 2,
        "text": "Hello Dobot."
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
