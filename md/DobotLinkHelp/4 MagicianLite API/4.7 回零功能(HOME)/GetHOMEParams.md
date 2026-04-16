### 4.7.2 GetHOMEParams

**获取回零参数**

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

响应参数 result

</div>

<div>

  ------- -------- ------------ --------------
  字段   类型   是否必填   说明
  x      float   是          当前x的位置
  y      float   是          当前y的位置
  z      float   是          当前z的位置
  r      float   是          当前r的位置
  ------- -------- ------------ --------------

</div>

**KeyWords:**

portName: string

x: float

y: float

z: float

r: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetHOMEParams",
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
        "x": 192.88986206054688,
        "y": 23.918956756591797,
        "z": 67.55459594726562,
        "r": 7.06879997253418
    }
}
```
