### 5.12.1 GetColorObjExist

**获取存在的颜色对象**

请求参数 params

  ----------- --------- ----------- -------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号(0~5)
  color      int      是         颜色标识（1~7）
  ----------- --------- ----------- -------------------

响应参数 result

  --------- -------- ------------ -----------------------------------
  字段     类型   是否必填   说明
  status   int     是          检测状态，True检测到/False未检测
  --------- -------- ------------ -----------------------------------

**KeyWords:**

portName: string

port: int (0~5，端口号)

color: int (1~7，颜色标识)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetColorObjExist",
    "params": {
        "portName": "COM4",
        "port": 0,
        "color": 1
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "status": 0
 }
}
```
