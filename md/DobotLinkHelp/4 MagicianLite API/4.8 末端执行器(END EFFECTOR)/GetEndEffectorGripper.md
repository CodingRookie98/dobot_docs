### 4.8.8 GetEndEffectorGripper

**获取爪子输出**

<div>

请求参数 params

</div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

  ----------- --------- ------------ -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ------------ -----------

<div>

响应参数 result

</div>

  ------------ -------- ------------- ---------------------------------------
  字段        类型   是否必填   说明
  isEnabled   bool    是           控制是否使能 （true：是，false：否）
  isOn        bool    是           爪子是否抓住（true：是，false：否）
  ------------ -------- ------------- ---------------------------------------

**KeyWords:**

portName: string

isEnabled: bool

isOn: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorGripper",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "isEnabled": false,
 "isOn": false
 }
}
```
