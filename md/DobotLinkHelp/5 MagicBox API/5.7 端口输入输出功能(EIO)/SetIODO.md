### 5.7.3 SetIODO

[**设置I/O口输出电平**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

请求参数 params

  ----------- --------- ------------ --------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  port       int      是          EIO地址（0~25）
  level      int      是          输出电平（0：低电平，1：高电平）
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

level: int (0~1)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetIODO",
    "params": {
        "portName": "COM4",
        "port": 1,
        "level": 1,
        "isQueued": false
    }
}
```
