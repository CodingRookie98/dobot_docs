### 5.7.14 GetInfraredSensor

**获取红外传感器**

请求参数 params

  ----------- --------- ------------ ---------------
  字段       类型    是否必填   说明
  portName   string   是         通信端口
  port       int      是          要使能的端口
  ----------- --------- ------------ ---------------

<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- -------------------------------------
  字段     类型   是否必填   说明
  status   int     是         响应结果（0:获取失败，1:获取成功）
  --------- ------- ----------- -------------------------------------

</div>

**KeyWords:**

portName: string

port: int (0~25)

status: int (0~1)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetInfraredSensor",
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
 "status": 1
 }
}
```
