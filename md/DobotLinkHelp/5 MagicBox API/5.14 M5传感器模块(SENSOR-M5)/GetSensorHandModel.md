### 12.1.33 GetSensorHandModel

**获取手势识别模块**

请求参数 params

  ----------- --------- ----------- -----------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         端口号（0~5）
  ----------- --------- ----------- -----------------

响应参数 result

+-----------------+-----------------+-----------------+-----------------+
| 字段           | 类型           | 是否必填       | 说明           |
+-----------------+-----------------+-----------------+-----------------+
| data           | string         | 是             | 识别值：        |
|                 |                 |                 |                 |
|                 |                 |                 | 返回            |
|                 |                 |                 | 值的每个位数代  |
|                 |                 |                 | 表一个手势位置  |
|                 |                 |                 |                 |
|                 |                 |                 | ( // REGISTER 0 |
|                 |                 |                 |                 |
|                 |                 |                 | GES_RIGHT_FLAG  |
|                 |                 |                 | = BIT(0),       |
|                 |                 |                 |                 |
|                 |                 |                 | GES_LEFT_FLAG = |
|                 |                 |                 | BIT(1),         |
|                 |                 |                 |                 |
|                 |                 |                 | GES_UP_FLAG =   |
|                 |                 |                 | BIT(2),         |
|                 |                 |                 |                 |
|                 |                 |                 | GES_DOWN_FLAG = |
|                 |                 |                 | BIT(3),         |
|                 |                 |                 |                 |
|                 |                 |                 | G               |
|                 |                 |                 | ES_FORWARD_FLAG |
|                 |                 |                 | = BIT(4),       |
|                 |                 |                 |                 |
|                 |                 |                 | GE              |
|                 |                 |                 | S_BACKWARD_FLAG |
|                 |                 |                 | = BIT(5),       |
|                 |                 |                 |                 |
|                 |                 |                 | GES             |
|                 |                 |                 | _CLOCKWISE_FLAG |
|                 |                 |                 | = BIT(6),       |
|                 |                 |                 |                 |
|                 |                 |                 | GES_COUNT       |
|                 |                 |                 | _CLOCKWISE_FLAG |
|                 |                 |                 | = BIT(7),       |
|                 |                 |                 |                 |
|                 |                 |                 | // REGISTER 1   |
|                 |                 |                 |                 |
|                 |                 |                 | GES_WAVE_FLAG = |
|                 |                 |                 | BIT(0),         |
|                 |                 |                 | READ_ERR =      |
|                 |                 |                 | 0xff）          |
+-----------------+-----------------+-----------------+-----------------+

**KeyWords:**

portName: string

port: int, 端口，0~5

data: int

// REGISTER 0

GES_RIGHT_FLAG = BIT(0), GES_LEFT_FLAG = BIT(1), GES_UP_FLAG = BIT(2),
GES_DOWN_FLAG = BIT(3), GES_FORWARD_FLAG = BIT(4), GES_BACKWARD_FLAG =
BIT(5), GES_CLOCKWISE_FLAG = BIT(6), GES_COUNT_CLOCKWISE_FLAG = BIT(7),

// REGISTER 1

GES_WAVE_FLAG = BIT(0), READ_ERR = 0xff,

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetSensorHandModel",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "data": 255
 }
}
```
