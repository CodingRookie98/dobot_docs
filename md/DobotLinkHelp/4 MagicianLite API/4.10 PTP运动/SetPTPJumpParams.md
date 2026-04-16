### 4.10.7 SetPTPJumpParams

[**设置门型模式点位参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

[请求参数
params]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

  ------------- --------- ------------ --------------
  字段         类型    是否必填   说明
  portName     string   是          通信端口
  zLimit       float    是          门型模式运动最大抬升高度限制
  jumpHeight   float    是          门型模式运动抬升距离
  isQueued     bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ------------- --------- ------------ --------------
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

zLimit: float

jumpHeight: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetPTPJumpParams",
    "params": {
        "portName": "COM4",
        "zLimit": 100,
        "jumpHeight": 20,
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
