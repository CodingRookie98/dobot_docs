### 12.1.31 SensorSetSYNCmd

**语音模块控制命令**

请求参数 params

  ----------- --------- ----------- --
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（1）
  cmd        int      是         语音命令（0：停止播放，1：暂停播放，2：继续播放，3：下一曲，4：上一曲）
  ----------- --------- ----------- --
响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

port: int (1)

cmd: int (0:stop 1:suspend 2:resume 3:next 4:previous)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetSYNCmd",
    "params": {
        "portName": "COM4",
        "port": 1,
        "cmd": 0
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
