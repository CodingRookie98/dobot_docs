### 12.1.28 SensorSetSYN

**设置语音播放音量和速度**

请求参数 params

  ----------- --------- ----------- --------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（1）
  sound      int      是         音量:0~15
  speed      int      是          速度:0~5
  ----------- --------- ----------- --------------

响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

port: int (1)

sound: int (音量:0~15)

speed: int (速度:0~5)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetSYN",
    "params": {
        "portName": "COM4",
        "port": 1,
        "sound": 5,
        "speed": 1
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
