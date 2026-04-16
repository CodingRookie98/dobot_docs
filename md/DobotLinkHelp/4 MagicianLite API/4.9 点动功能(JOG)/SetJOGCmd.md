### 4.9.7 SetJOGCmd

[执行点动功能]{style="FONT-SIZE: 14.05pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ------------ -----------------------------------------------------------------------------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  isJoint    bool     是          点动方式 （false：坐标轴点动 true：关节点动）
  cmd        int      是          点动命令（0：停止执行、1：x正方向运行、2：x反方向运行、3：y正反向运行、4：y反方向运行、5：z正方向运行、6：z反方向运行、7：r正方向运行、8：r反方向运行）
  isQueued   bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ------------ -----------------------------------------------------------------------------------
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

isJoint: bool

cmd: int (0:stop X:1,2 Y:3,4 Z:5,6 R:7,8)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetJOGCmd",
    "params": {
        "portName": "COM4",
        "isJoint": false,
        "cmd": 2,
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
