### 5.5.1 GetPoseL

<div>

[**获取滑轨实时位姿**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

<div>

响应参数 result

</div>

<div>

</div>

<div>

</div>

<div>

  ------------ ------- ----------- ----------
  字段        类型   是否必填   说明
  positionL   float   是         滑轨位置
  ------------ ------- ----------- ----------

</div>

**KeyWords:**

portName: string

positionL: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetPoseL",
    "params": {
        "portName": "COM4",
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "positionL": 0
 }
}
```
