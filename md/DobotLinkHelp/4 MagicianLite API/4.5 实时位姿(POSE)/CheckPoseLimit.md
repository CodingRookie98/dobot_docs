### 4.5.3 CheckPoseLimit

**检查点位限制**

请求参数 Params

  ----------- --------- ------------ ------------------------------------------------------
  字段       类型   是否必填   说明
  portName   string   是          通信端口
  isJoint    bool     是          控制方式（true表示关节坐标系，下面x、y、z、r对应j1、j2、j3、j4，false表示笛卡尔坐标系,x y z r就是x y z r）
  x          float    是          当前x的位置（ [-135°~135°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
  y          float    是          当前y的位置（ [-5°~80°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
  z          float    是          当前z的位置（ [-10°~85°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
  r          float    是          当前r的位置（ [-145°~145°]{style="FONT-SIZE: 9pt; FONT-FAMILY: Times New Roman; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}）
  ----------- --------- ------------ ------------------------------------------------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  ------------ ------- ----------- ---------------------------------------------
  字段        类型   是否必填   说明
  isLimited   bool    是         响应结果（true：操作成功，false：操作失败）
  ------------ ------- ----------- ---------------------------------------------

</div>

**KeyWords:**

portName: string

isJoint: bool (default:false)

x: float

y: float

z: float

r: float

isLimited: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.CheckPoseLimit",
    "params": {
        "portName": "COM4",
        "isJoint": false,
        "x": 100.6,
        "y": 260.0,
        "z": 20.0,
        "r": 0.0
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "isLimited": false
 }
}
```
