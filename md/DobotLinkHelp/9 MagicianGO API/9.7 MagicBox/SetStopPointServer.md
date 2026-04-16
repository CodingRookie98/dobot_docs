### 9.8.1 SetStopPointServer

**开启自动停车服务，传入一个点，当车辆行驶到点时，自动停车**

请求参数 params

  ----------- --------- ----------- ----------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  PointX     int      是         停车点的X坐标
  PointY     int      是         停车点的Y坐标
  ----------- --------- ----------- ----------------

响应参数 result

  --------- -------- ------------ --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是          响应结果（true:操作成功，false:操作失败）
  --------- -------- ------------ --------------------------------------------

**KeyWords:**

portName: string

PointX: int，停车点的X坐标

PointY: int，停车点的Y坐标

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetStopPointServer",
    "params": {
        "portName": "COM4",
        "PointX" : 10,
        "PointY" : 10
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
