### 4.8.3 SetEndEffectorType

**设置末端配件类型**

<div>

请求参数 params

</div>

  ----------- ---------- ------------ -------------
  字段      类型     是否必填   说明
  portName   string   是          通信端口
  type       int      是          末端配件类型（0：无配件，1：吸盘配件，2：爪子配件，3：笔配件）
  isQueued   bool      否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行）默认：false
  ----------- ---------- ------------ -------------
<div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- ----------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true：操作成功，false：操作失败）
  --------- ------- ----------- ----------------------------------------------

</div>

</div>

**KeyWords:**

portName: string

type: int (0:None 1:SucktionCup 2:Gripper 3:Pen)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetEndEffectorType",
    "params": {
        "portName": "COM4",
        "type": 1,
        "isQueued": false
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
