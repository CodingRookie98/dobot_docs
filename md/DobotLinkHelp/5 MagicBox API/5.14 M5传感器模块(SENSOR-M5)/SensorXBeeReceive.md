### 12.1.25 SensorXBeeReceive

**XBee 接收**

请求参数 params

  ----------- --------- ----------- ------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号(2)
  ----------- --------- ----------- ------------

响应参数 result

  ------- --------- ------------ ------------
  字段   类型    是否必填   说明
  text   string   是          接收字符串
  ------- --------- ------------ ------------

**KeyWords:**

portName: string

port: int (2)

text: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorXBeeReceive",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "text": ""
 }
}
```
