### 9.8.2 SetStopPointParam

**设置自动停车服务参数**

请求参数 params

  ----------- --------- ----------- -----------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  scopeErr   int      是         进入停车范围，默认参数40cm
  stopErr    int      是         停车的精确度，默认参数2cm
  ----------- --------- ----------- -----------------------------

响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

scopeErr: int, 进入停车范围，默认参数40cm

stopErr: int, 停车的精确度，默认参数2cm

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetStopPointParam",
    "params": {
        "portName": "COM4",
        "scopeErr": 40,
        "stopErr" : 2
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
