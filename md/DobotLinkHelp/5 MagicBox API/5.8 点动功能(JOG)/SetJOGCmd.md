### 5.8.1 SetJOGCmd

**执行点动动能**

请求参数 params

  ----------- --------- ----------- --------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  isJoint    bool     是         点动方式（0：坐标轴点动，1：关节点动）
  cmd        int      是         点动命令（取值：9,10）
  isQueued   bool     否        队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ----------- --------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

</div>

**KeyWords:**

portName: string

isJoint: bool

cmd: int (L:9,10)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetJOGCmd",
    "params": {
        "portName": "COM4",
        "isJoint": true,
        "cmd": 9,
        "isQueued": false
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
