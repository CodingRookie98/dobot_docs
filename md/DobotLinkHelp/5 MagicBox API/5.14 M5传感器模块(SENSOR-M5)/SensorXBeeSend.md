### 12.1.24 SensorXBeeSend

**XBee 发送**

请求参数 params

  ----------- --------- ----------- --------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（2）
  text       string   是         发送字符串
  ----------- --------- ----------- --------------

响应参数 result

  --------- -------- ------------ -------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ -------------------------------------------

**KeyWords:**

portName: string

port: int (2)

text: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorXBeeSend",
    "params": {
        "portName": "COM4",
        "port": 2,
        "text": "led1 on, ..."
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
