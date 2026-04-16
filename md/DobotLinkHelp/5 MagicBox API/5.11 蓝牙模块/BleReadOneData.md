### 5.11.5 BleReadOneData

**蓝牙数据接收，仅适用于蓝牙主机模式，只接收一个数据**

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

响应参数 result

  ------- ------- ----------- ------------
  字段   类型   是否必填   说明
  data   int    是         数据内容
  ------- ------- ----------- ------------

**KeyWords:**

portName: string

data: int,数据内容

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleReadOneData",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT：

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.BleReadOneData",
    "params": {
        "data": 1
    }
}
```
