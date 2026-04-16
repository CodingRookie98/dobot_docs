### 4.8.2 GetEndEffectorParams

**获取末端执行器操作**

<div>

请求参数 params

</div>

<div>

</div>

<div>

  ----------- --------- ----------- ----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- ----------

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

  ---------- -------- ------------ ------------------
  字段      类型   是否必填   说明
  xOffset   int     是          末端x轴方向长度
  yOffset   int     是          末端y轴方向长度
  zOffset   int     是          末端z轴方向长度
  ---------- -------- ------------ ------------------

**KeyWords:**

portName: string

xOffset: float

yOffset: float

zOffset: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorParams",
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
 "xOffset": 57,
 "yOffset": 0,
 "zOffset": 0
 }

}
```
