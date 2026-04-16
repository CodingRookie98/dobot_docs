### 4.4.2 GetArmSpeedRatio

**获取机械臂速度**

请求参数 params

  ----------- --------- ----------- -----------------------------------------------
  字段       类型     是否必填   说明
  portName   string   是          设备的通信端口
  type       int       是         运动类型（0：点动速度，1：点到点的运动速度）
  ----------- --------- ----------- -----------------------------------------------

响应结果 result

  -------- ------- ----------- -------
  字段    类型   是否必填   说明
  type    int    是          设备的通信端口
  value   int     是         [运动速度]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri"} (0~100 unit:%)
  -------- ------- ----------- -------
**KeyWords:**

portName: string

type : int (0:JOG 1:PTP)

value: int (0~100 unit:%)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetArmSpeedRatio",
    "params": {
        "portName": "COM4",
        "type": 1
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "type": 1,
 "value": 0
 }

}
```
