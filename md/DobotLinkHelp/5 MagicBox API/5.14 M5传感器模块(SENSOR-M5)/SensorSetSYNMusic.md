### 12.1.29 SensorSetSYNMusic

**设置语音播放音乐**

请求参数 params

  ----------- --------- ----------- -------------------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（1）
  type       int      是         语音类型(0:背景音 1:音效 2:提示音)
  index      int      是         语音索引
  ----------- --------- ----------- -------------------------------------

响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

port: int (1)

type: int (0:背景音 1:音效 2:提示音)

index: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetSYNMusic",
    "params": {
        "portName": "COM4",
        "port": 1,
        "type": 0,
        "index": 2
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
