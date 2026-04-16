### 4.9.3 SetJOGCoordinateParams

[**设置坐标系参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

<div>

请求参数 params

</div>

<div>

</div>

  --------------- --------------- ------------ ------------------------------------------------------------
  字段           类型          是否必填   说明
  portName       string         是          通信端口
  velocity       array(float)   是          [4 轴坐标轴（x,y,z,r）速度 (取值范围：0-225) ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  acceleration   array(float)   是          [4 轴坐标轴（x,y,z,r）加速度(取值范围：0-100) ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  isQueued       bool           否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  --------------- --------------- ------------ ------------------------------------------------------------
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
    "method": "dobotlink.MagicianLite.SetJOGCoordinateParams",
    "params": {
        "portName": "COM4",
        "velocity": [60, 60, 60, 60],
        "acceleration": [60, 60, 60, 60],
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
