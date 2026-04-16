### 5.7.5 SetIOPWM

**设置I/O PWM输出**

请求参数 params

  ------------ --------- ----------- --------------
  字段        类型     是否必填   说明
  portName    string   是         通信端口
  port        int      是         EIO地址（0~25）
  frequency   float    是         PWM 频率 (10Hz~1MHz)
  dutyCycle   float    是         PWM 占空比 0~100
  isQueued    bool     否         队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ------------ --------- ----------- --------------
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

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetIOPWM",
    "params": {
        "portName": "COM4",
        "port": 1,
        "frequency": 10.2,
        "dutyCycle": 30.0,
        "isQueued": false
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0".

 "result": true
 }
```
