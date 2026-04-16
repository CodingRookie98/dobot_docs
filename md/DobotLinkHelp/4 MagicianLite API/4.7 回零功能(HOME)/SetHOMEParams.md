### 4.7.1 SetHOMEParams

[设置回零参数]{style="FONT-SIZE: 15pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

<div>

请求参数 params

</div>

<div>

</div>

<div>

  ----------- --------- ------------ -------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  x          float    是          当前x的位置
  y          float    是          当前y的位置
  z          float    是          当前z的位置
  r          float    是          当前r的位置
  isQueued   bool     是          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行）默认：false
  ----------- --------- ------------ -------------
</div>

<div>

</div>

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

x: float

y: float

z: float

r: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetHOMEParams",
    "params": {
        "portName": "COM4",
        "x": 20.65,
        "y": 5.84,
        "z": 2.36,
        "r": 0.0,
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
