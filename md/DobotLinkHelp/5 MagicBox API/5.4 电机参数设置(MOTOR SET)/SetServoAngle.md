### 5.4.1 SetServoAngle

[**设置舵机的角度**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 Params

  ----------- --------- ------------ -------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  index      int      是          舵机序号：端口号 0-5
  value      float    是          角度值 (+/-180)
  isQueued   bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ------------ -------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  -------- ------- ----------- ----------------------
  字段    类型   是否必填   说明
  angle   int     是          角度值 (+/-180)
  index   int     是         舵机序号：端口号 0-5
  -------- ------- ----------- ----------------------

</div>

**KeyWords:**

portName: string

index: int

value: float (+/-180)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetServoAngle",
    "params": {
        "portName": "COM4",
        "index": 2,
        "value": 60,
        "isQueued": false
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "angle": 60,
 "index": 2
 }
}
```
