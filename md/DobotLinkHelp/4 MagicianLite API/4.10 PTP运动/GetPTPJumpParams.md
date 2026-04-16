### 4.10.8 GetPTPJumpParams

<div>

[**获取门型模式点位参数**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

请求参数 params

</div>

  ----------- --------- ------------ -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ------------ -----------

<div>

响应参数 result

</div>

  ------------- -------- ------------ ------------------------------
  字段        类型    是否必填   说明
  jumpHeight   float   是          门型模式运动抬升距离
  zLimit       float   是          门型模式运动最大抬升高度限制
  ------------- -------- ------------ ------------------------------

**KeyWords:**

portName: string

zLimit: float

jumpHeight: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPTPJumpParams",
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
 "jumpHeight": 20,
 "zLimit": 100
 }

}
```
