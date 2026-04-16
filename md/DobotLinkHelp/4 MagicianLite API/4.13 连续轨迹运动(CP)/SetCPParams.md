### 4.13.1 SetCPParams

[**设置连续轨迹运动参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ------------------ --------- ------------ --------------------------------------------------
  字段              类型    是否必填   说明
  portName          string   是          通信端口
  targetAcc         float    是          [规划加速度最大值 ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  junctionVel       float    是          [拐角加速度最大值]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  isRealTimeTrack   bool     是          是否开启实时模式（ true: 是 false: 否）
  acc               float    否          [实际加速度最大值，非实时模式下使用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  period            float    否          [插补周期，实时模式下使用 ]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  isQueued          bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ------------------ --------- ------------ --------------------------------------------------
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

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float(isRealTimeTrack = false)

*period: float(isRealTimeTrack = true)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCPParams",
    "params": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100,
        "isQueued": false
    }
}
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetCPParams",
    "params": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": true,
        "period": 20,
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
