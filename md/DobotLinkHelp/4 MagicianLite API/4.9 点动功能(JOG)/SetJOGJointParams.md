### 4.9.1 SetJOGJointParams

[**设置关节点动参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

<div>

请求参数 params

</div>

  --------------- --------------- ------------ --------------
  字段          类型          是否必填   说明
  portName       string         是          通信端口
  velocity       array(float)   是          4 轴关节速度
  acceleration   array(float)   是          4 轴关节加速度
  isQueued       bool           否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  --------------- --------------- ------------ --------------
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

velocity: array(float)

acceleration: array(float)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetJOGJointParams",
    "params": {
        "portName": "COM4",
        "velocity": [15, 15, 15, 30],
        "acceleration": [50, 50, 50, 50],
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
