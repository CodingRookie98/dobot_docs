### 5.11.8 BleReadMeshData

**蓝牙组网模式数据接收**

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

响应参数 result

  -------- --------- ------------ ----------------------------
  字段    类型    是否必填   说明
  state   int      是          0-接收成功，其他-接收失败
  devID   int      是          发送者ID
  data    string   是          数据内容
  -------- --------- ------------ ----------------------------

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleReadMeshData",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
           "state": 0 , //0-接收成功，其他-接收失败
           "devID": 123 ,  //发送者ID
           "data": "string"     //数据内容
    }
}
```
