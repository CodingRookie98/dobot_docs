### 5.7.6 GetIOPWM

**获取I/O PWM输出**

请求参数 params

  ----------- --------- ----------- -------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是         EIO地址（0~25）
  ----------- --------- ----------- -------------------

响应参数 result

  ------------ -------- ------------ ------------------------
  字段       类型    是否必填   说明
  dutyCycle   float   是          PWM 占空比 0~100
  frequency   float   是          PWM 频率 (10Hz~1MHz)
  port        int     是          EIO地址（0~25）
  ------------ -------- ------------ ------------------------

**KeyWords:**

portName: string

port: int (0~25)

frequency: float (10Hz~1MHz)

dutyCycle: float (0~100)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetIOPWM",
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
 "dutyCycle": 30,
 "frequency": 10.199999809265137,
 "port": 1
 }
}
```
