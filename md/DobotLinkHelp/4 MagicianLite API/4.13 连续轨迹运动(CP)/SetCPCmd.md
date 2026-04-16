### 4.13.3 SetCPCmd

[**执行连续轨迹功能**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ------------ --------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  cpMode     int      是          CP模式（0：相对模式 1：绝对模式 ）
  x          float    是          x 坐标增量 / x 轴坐标
  y          float    是          y 坐标增量 / y 轴坐标
  z          float    是          z 坐标增量 / z 轴坐标
  power      float    是          激光功率
  isQueued   bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ------------ --------------
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

cpMode: int (0~1)

x: float

y: float

z: float

power: float

*isQueued: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCPCmd",
    "params": {
        "portName": "COM4",
        "cpMode": 0,
        "x": 20.0,
        "y": 5.0,
        "z": 1.0,
        "power": 20.0,
        "isQueued": true
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
