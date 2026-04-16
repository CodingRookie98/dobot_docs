### 5.7.13 SetInfraredSensor

**设置红外传感器**

请求参数 params

  ----------- --------- ------------ --------------
  字段       类型    是否必填   说明
  portName   string   是         通信端口
  port       int      是          要使能的端口(0~25)
  enable     bool     是          是否使能（true:是，false:否）
  version    int      是          要使用的传感器版本
  isQueued   bool     否          队列指令（true：指令排队执行，false：打断当前执行的任务，直接插入执行 ）默认：false
  ----------- --------- ------------ --------------
<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

</div>

**KeyWords:**

portName: string

port: int (0~25)

enable: bool

version: int

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetInfraredSensor",
    "params": {
        "portName": "COM4",
        "port": 1,
        "enable": true,
        "version": 1,
        "isQueued": false
    }
}
```
