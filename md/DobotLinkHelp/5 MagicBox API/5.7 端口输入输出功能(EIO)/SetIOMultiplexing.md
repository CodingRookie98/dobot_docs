### 5.7.1 SetIOMultiplexing

**设置IO复用**

请求参数 params

+-----------------+-----------------+-----------------+-----------------+
| 字段           | 类型          | 是否必填      | 说明          |
+-----------------+-----------------+-----------------+-----------------+
| portName       | string         | 是             | 通信端口       |
+-----------------+-----------------+-----------------+-----------------+
| port           | int            | 是             | E               |
|                 |                 |                 | IO地址（0~25） |
+-----------------+-----------------+-----------------+-----------------+
| multiplex      | int            | 是             | 复用功能：（  |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 0：IOF          |
|                 |                 |                 | unctionDumm：不 |
|                 |                 |                 | 配置功能，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | []{sty          |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 | [               |
|                 |                 |                 | 1：IOFunctionDO |
|                 |                 |                 | ：IO输出，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 2：             |
|                 |                 |                 | IOFunctionPWM： |
|                 |                 |                 | PWM输出，]{sty  |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 3：IOFunctionDI |
|                 |                 |                 | ：IO输入，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [               |
|                 |                 |                 | 4               |
|                 |                 |                 | ：IOFunctionADC |
|                 |                 |                 | ：AD输入，]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [5：IOFunctionD |
|                 |                 |                 | IPU：上拉输入， |
|                 |                 |                 | ]{sty           |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [6：I           |
|                 |                 |                 | OFunctionDIPD： |
|                 |                 |                 | 下拉输入。]{sty |
|                 |                 |                 | le="FONT-SIZE:  |
|                 |                 |                 | 9pt; FONT-FAMIL |
|                 |                 |                 | Y: Times New Ro |
|                 |                 |                 | man; COLOR: rgb |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
|                 |                 |                 |                 |
|                 |                 |                 | ）              |
+-----------------+-----------------+-----------------+-----------------+
| isQueued       | bool           | 否             | 队列指令（t    |
|                 |                 |                 | rue：指令排队执 |
|                 |                 |                 | 行，false：打断 |
|                 |                 |                 | 当前执行的任务  |
|                 |                 |                 | ，直接插入执行  |
|                 |                 |                 | ）默认：false   |
+-----------------+-----------------+-----------------+-----------------+

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

multiplex: int (0~6)

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetIOMultiplexing",
    "params": {
        "portName": "COM4",
        "port": 1,
        "multiplex": 1,
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
