### 4.8.6 GetEndEffectorSuctionCup

**获取吸盘吸放状态**

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

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

  ------------ ------- ------------ ---------------------------------------
  字段       类型   是否必填   说明
  isEnabled   bool   是          控制是否使能 （true：是，false：否）
  isOn        bool   是          吸盘是否吸住（true：是，false：否）
  ------------ ------- ------------ ---------------------------------------

**KeyWords:**

portName: string

isEnabled: bool

isOn: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorSuctionCup",
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
 "isOn": true

   }

 }
```
