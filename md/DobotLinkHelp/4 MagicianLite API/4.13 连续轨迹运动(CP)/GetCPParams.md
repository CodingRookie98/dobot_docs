### 4.13.2 GetCPParams

[**获取连续运动轨迹参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

<div>

响应参数 result

</div>

  ------------------ --------- ------------ --------------------------------------------------
  字段              类型    是否必填   说明
  portName          string   是          通信端口
  targetAcc         float    是          [规划加速度最大值]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  junctionVel       float    是           [ 拐角加速度最大值]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体;
                                            COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  isRealTimeTrack   bool     是          是否开启实时模式（ true: 是 false: 否）
  acc               float    否          [实际加速度最大值，非实时模式下使用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  period            float    否          [插补周期，实时模式下使用]{style="FONT-SIZE: 9pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}
  ------------------ --------- ------------ --------------------------------------------------
**KeyWords:**

portName: string

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float(isRealTimeTrack = false)

*period: float(isRealTimeTrack = true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetCPParams",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100
    }
}
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "isRealTimeTrack": true,
 "junctionVel": 100,
 "period": 20,
 "targetAcc": 200
 }

}
```
