### 12.1.30 SensorSendSYN

**设置语音模块播放合成语音**

注：使用该接口前，需先使用SensorSYNInit接口

请求参数 params

  ----------- --------- ----------- --------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（1）
  text       string   是         合成的音效
  ----------- --------- ----------- --------------

响应参数result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

port: int (1)

text: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSendSYN",
    "params": {
        "portName": "COM4",
        "port": 1,
        "text": "..."
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
