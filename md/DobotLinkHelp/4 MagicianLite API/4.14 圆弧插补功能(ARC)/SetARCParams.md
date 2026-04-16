### 4.14.1 SetARCParams

<div>

[**设置圆弧插补功能参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ------------------ --------- ------------ --------------
  字段             类型    是否必填   说明
  portName          string   是          通信端口
  xyzVelocity       float    是          圆弧运动 xyz 三坐标轴速度
  rVelocity         float    是          圆弧运动末端旋转速度
  xyzAcceleration   float    是          圆弧运动 xyz 三坐标轴加速度
  rAcceleration     float    是          圆弧运动末端旋转加速度
  isQueued          bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ------------------ --------- ------------ --------------
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

**KeyWords:**

portName: string

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetARCParams",
    "params": {
        "portName": "COM4",
        "xyzVelocity": 200,
        "rVelocity": 200,
        "xyzAcceleration": 200,
        "rAcceleration": 200,
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
