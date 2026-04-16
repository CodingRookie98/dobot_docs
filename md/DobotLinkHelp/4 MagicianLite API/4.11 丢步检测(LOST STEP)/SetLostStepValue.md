### 4.11.1 SetLostStepValue

<div>

[设置丢步检测功能]{style="FONT-SIZE: 14.05pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

<div>

</div>

<div>

  ----------- --------- ------------ ------------------------
  字段      类型     是否必填   说明
  portName   string   是          通信端口
  value      float    是          丢步检测偏离值（8-15）
  ----------- --------- ------------ ------------------------

</div>

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

**KeyWords:**

portName: string

value: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetLostStepValue",
    "params": {
        "portName": "COM4",
        "value": 10
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
