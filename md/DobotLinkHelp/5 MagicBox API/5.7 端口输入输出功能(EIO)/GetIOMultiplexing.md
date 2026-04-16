### 5.7.2 GetIOMultiplexing

**获取IO复用**

请求参数 params

  ----------- --------- ------------ -------------------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  port       int      是          EIO地址（0~25）
  ----------- --------- ------------ -------------------

<div>

响应参数 result

</div>

+-----------------+-----------------+-----------------+-----------------+
| 字段           | 类型         | 是否必填      | 说明          |
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
|                 |                 |                 | []{styl         |
|                 |                 |                 | e="FONT-SIZE: 9 |
|                 |                 |                 | pt; FONT-FAMILY |
|                 |                 |                 | : Times New Rom |
|                 |                 |                 | an; COLOR: rgb( |
|                 |                 |                 | 0,0,0); mso-spa |
|                 |                 |                 | cerun: 'yes'"}[ |
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
|                 |                 |                 | [2：            |
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
|                 |                 |                 | [               |
|                 |                 |                 | 5：I            |
|                 |                 |                 | OFunctionDIPU： |
|                 |                 |                 | 上拉输入，]{sty |
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
|                 |                 |                 | 6：I            |
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
| port           | int            | 是             | E              |
|                 |                 |                 | IO地址（0~25） |
+-----------------+-----------------+-----------------+-----------------+

**KeyWords:**

portName: string

port: int (0~25)

multiplex: int (0~6)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOMultiplexing",
    "params": {
        "portName": "COM4",
        "port": 1
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "multiplex": 1,
 "port": 1
 }
}
```
