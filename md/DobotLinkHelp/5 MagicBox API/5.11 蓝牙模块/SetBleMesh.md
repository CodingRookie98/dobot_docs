### 5.11.7 SetBleMesh

**设置蓝牙组网模式 ，设置组网模式的组ID和当前设备ID。**

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  groupID    int      是         组ID
  devID      int      是         设备ID
  ----------- --------- ----------- -----------

响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

groupID: int,组ID，长度6个字节，每个数字范围0-9

devID: int,设备ID，长度1个字节，0-255

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetBleMesh",
    "params": {
        "portName": "COM4" ,
        "groupID": 123465,
        "devID": 123
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
