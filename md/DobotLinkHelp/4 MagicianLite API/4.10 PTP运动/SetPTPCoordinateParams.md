### 4.10.5 SetPTPCoordinateParams

<div>

[**设置坐标轴点位参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

+-----------------+-----------------+-----------------+-----------------+
| 字段          | 类型          | 是否必填       | 说明          |
+-----------------+-----------------+-----------------+-----------------+
| portName       | string          | 是             | 通信端口       |
+-----------------+-----------------+-----------------+-----------------+
| xyzVelocity    | float          | 是             | PTP 模式下 xyz |
|                 |                 |                 | 3 轴坐标轴速度  |
+-----------------+-----------------+-----------------+-----------------+
| rVelocity      | float          | 是             | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [PTP           |
|                 |                 |                 | 模式下末端速度  |
|                 |                 |                 | ]{style="F      |
|                 |                 |                 | ONT-SIZE: 9pt;  |
|                 |                 |                 | FONT-FAMILY: 宋 |
|                 |                 |                 | 体; COLOR: rgb  |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
+-----------------+-----------------+-----------------+-----------------+
|                | float          | 是             | PTP 模式下 xyz |
| xyzAcceleration |                 |                 | 3               |
|                 |                 |                 | 轴坐标轴加速度  |
+-----------------+-----------------+-----------------+-----------------+
| rAcceleration  | float          | 是             | PTP            |
|                 |                 |                 | 模              |
|                 |                 |                 | 式下末端加速度  |
+-----------------+-----------------+-----------------+-----------------+
| isQueued       | bool           | 否             | 队列指令（t    |
|                 |                 |                 | rue：指令排队执 |
|                 |                 |                 | 行，false：打断 |
|                 |                 |                 | 当前执行的任务  |
|                 |                 |                 | ，直接插入执行  |
|                 |                 |                 | ）默认：false   |
+-----------------+-----------------+-----------------+-----------------+

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

xyzVelocity: float

rVelocity: float

xyzAcceleration: float

rAcceleration: float

*isQueued: bool (default:false)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetPTPCoordinateParams",
    "params": {
        "portName": "COM4",
        "xyzVelocity": 200,
        "rVelocity": 100,
        "xyzAcceleration": 200,
        "rAcceleration": 100,
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
