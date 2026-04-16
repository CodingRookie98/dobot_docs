### 5.12.2 GetColorObjCoordinate

**获取颜色坐标**

请求参数 params

  ------------- --------- ----------- -----------------
  字段         类型     是否必填   说明
  portName     string   是         通信端口
  port         int      是         端口号(0~5)
  color        int      是         颜色标识(1~7)
  coordinate   int      是         坐标
  ------------- --------- ----------- -----------------

响应参数 result

  ------------- ------- ----------- ----------
  字段         类型   是否必填   说明
  color        int    是         颜色标识
  coordinate   int    是         坐标
  ------------- ------- ----------- ----------

**KeyWords:**

portName: string

port: int (0~5，端口号)

color: int (1~7，颜色标识)

coordinate: int (1~4, 1代表x,2代表y,3代表l,4代表z)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetColorObjCoordinate",
    "params": {
        "portName": "COM4",
        "port": 2,
        "color": 1,
        "coordinate": 1
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "color": 1,
 "coordinate": 0
 }
}
```
