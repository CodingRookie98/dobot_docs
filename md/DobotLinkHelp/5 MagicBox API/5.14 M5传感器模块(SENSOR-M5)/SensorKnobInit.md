### 12.1.8 SensorKnobInit

**初始化电位器**

请求参数

  ----------- --------- ------------ ----------------
  字段      类型    是否必填   说明
  portName   string   是          通信端口
  port       int      是          端口号 (2~3)
  ----------- --------- ------------ ----------------

响应参数

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

**KeyWords:**

portName: string

port: int (2~3)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorKnobInit",
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
 "result": true
}
```
