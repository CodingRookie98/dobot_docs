### 4.8.4 GetEndEffectorType

**获取末端配件类型**

<div>

请求参数 params

</div>

<div>

</div>

<div>

  ----------- --------- ----------- ----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- ----------

</div>

<div>

</div>

<div>

<div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

  ------- ------- ----------- ------------------------------------------------------------
  字段   类型   是否必填   说明
  type   int     是         响应结果（0:没配件，1：吸盘配件，2：爪子配件，3：笔配件）
  ------- ------- ----------- ------------------------------------------------------------

</div>

</div>

</div>

**KeyWords:**

portName: string

type: int (0:None 1:SucktionCup 2:Gripper 3:Pen)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorType",
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
 "type": 1
 }
}
```
