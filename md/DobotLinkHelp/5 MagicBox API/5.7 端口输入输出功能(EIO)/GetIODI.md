### 5.7.7 GetIODI

**读取I/O 输入电平**

请求参数 params

  ----------- --------- ----------- -------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         EIO地址（0~25）
  ----------- --------- ----------- -------------------

相应参数 result

  -------- ------- ----------- -----------------------------------
  字段    类型   是否必填   说明
  level   int    是         输出电平（0：低电平，1：高电平）
  port    int    是         EIO地址（0~25）
  -------- ------- ----------- -----------------------------------

**KeyWords:**

portName: string

port: int (0~25)

level: int (0~1)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIODI",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
    "result": {
 "level": 0,
 "port": 1
 }
}

```
