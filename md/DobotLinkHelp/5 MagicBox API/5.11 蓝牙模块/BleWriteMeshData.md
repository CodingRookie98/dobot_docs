### 5.11.9 BleWriteMeshData

**蓝牙组网模式数据发送**

请求参数 params

  ----------- --------- ----------- ------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  devID      int      是         发送者ID
  data       string   是         数据内容
  ----------- --------- ----------- ------------

响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

devID: int，接收者ID

data: string，数据内容

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleWriteMeshData",
    "params": {
        "portName": "COM4",
        "devID": 123,
        "data": "string"
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
