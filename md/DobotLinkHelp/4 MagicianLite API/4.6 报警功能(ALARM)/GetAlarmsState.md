### 4.6.1 GetAlarmsState

[**获取报警状态**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

<div>

请求参数 params

</div>

<div>

</div>

<div>

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

</div>

<div>

</div>

<div>

</div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

+-----------------+-----------------+-----------------+-----------------+
| 字段           | 类型           | 是否必填       | 说明           |
+-----------------+-----------------+-----------------+-----------------+
| state          | array(int)      | 是             | <div>           |
|                 |                 |                 |                 |
|                 |                 |                 | [该数组存储每   |
|                 |                 |                 | 个报警项的报警  |
|                 |                 |                 | 状态（1：报警状 |
|                 |                 |                 | 态，0：非报警状 |
|                 |                 |                 | 态）]{style="F  |
|                 |                 |                 | ONT-SIZE: 9pt;  |
|                 |                 |                 | FONT-FAMILY: 楷 |
|                 |                 |                 | 体; COLOR: rgb  |
|                 |                 |                 | (0,0,0); mso-sp |
|                 |                 |                 | acerun: 'yes'"} |
|                 |                 |                 |                 |
|                 |                 |                 | </div>          |
+-----------------+-----------------+-----------------+-----------------+

</div>

**KeyWords:**

portName: string

state: array(int)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetAlarmsState",
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
        "state": [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    }
}
```
