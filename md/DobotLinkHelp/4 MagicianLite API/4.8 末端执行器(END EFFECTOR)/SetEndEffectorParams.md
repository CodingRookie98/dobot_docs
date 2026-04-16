### 4.8.1 SetEndEffectorParams

[**设置末端执行器参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

  ----------- --------- ------------ -------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  xOffset    float    是          末端x轴方向长度
  yOffset    float    是          末端y轴方向长度
  zOffset    float    是          末端z轴方向长度
  isQueued   bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行）默认：false
  ----------- --------- ------------ -------------
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

xOffset: float

yOffset: float

zOffset: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetEndEffectorParams",
    "params": {
        "portName": "COM4",
        "xOffset": 57.0,
        "yOffset": 0.0,
        "zOffset": 0.0,
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
