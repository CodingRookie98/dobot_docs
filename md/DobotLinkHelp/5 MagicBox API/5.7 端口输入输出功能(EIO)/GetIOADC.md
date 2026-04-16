### 5.7.8 GetIOADC

**读取I/O 模数转换值**

请求参数 params

  ----------- --------- ----------- -----------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         EIO地址(0~25)
  ----------- --------- ----------- -----------------

响应参数 result

  -------- ------- ----------- -----------------------
  字段    类型   是否必填   说明
  port    int    是         EIO地址(0~25)
  value   int    是         输入的ADC值(0~4095)
  -------- ------- ----------- -----------------------

**KeyWords:**

portName: string

port: int (0~25)

value: int (0~4095)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOADC",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "port": 1,
 "value": 0
 }
}
```
