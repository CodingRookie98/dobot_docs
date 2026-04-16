### 5.7.10 SetEMotorS

**设置扩展电机S的接口**

请求参数 params

  ----------- --------- ------------ --------------
  字段       类型     是否必填   说明
  portName   string   是          通信端口
  index      int      是          取值范围 0/1 （0-Stepper1，1-Stepper2）
  enable     bool     是          电机控制使能（false:不使能，true：使能）
  speed      int      是          电机控制速度（单位：脉冲个数每秒）
  distance   int      是          电机控制测量数据（单位：脉冲个数）
  isQueued   bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ------------ --------------
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

index: int (0~1)

enable: bool

speed: int (unit:pulse/sec)

distance: int (unit:pulse)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetEMotorS",
    "params": {
        "portName": "COM4",
        "index": 1,
        "enable": true,
        "speed": 250,
        "distance": 200,
        "isQueued": false
    }
}
```

OUTPUT:

```json
 {
 "id": 1,
 "jsonrpc": "2.0".
 "result": true
}
```
<div>

</div>
