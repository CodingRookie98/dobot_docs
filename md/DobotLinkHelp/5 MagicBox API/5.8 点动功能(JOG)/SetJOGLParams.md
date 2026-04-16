### 5.8.2 SetJOGLParams

**设置滑轨L点动参数**

请求参数 params

  --------------- --------- ----------- --------------
  字段           类型     是否必填   说明
  portName       string   是         通信端口
  velocity       float    是         滑轨关节速度
  acceleration   float    是         滑轨关节加速度
  isQueued       bool     否         队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  --------------- --------- ----------- --------------
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

velocity: float

acceleration: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetJOGLParams",
    "params": {
        "portName": "COM4",
        "velocity": 60,
        "acceleration": 60,
        "isQueued": false
    }
}
```
