### 12.1.22 SensorGetColorRes

**读取颜色识别结果**

注：使用该接口前，需先使用SensorColorInit接口

请求参数 params

  ----------- --------- ----------- ---------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  port       int      是        端口号(0~5)
  ----------- --------- ----------- ---------------

相应参数 result

  -------- -------- ----------- -------------------------------------------
  字段    类型    是否必填   说明
  color   string   是         颜色识别结果(none/red/green/blue/yellow)
  -------- -------- ----------- -------------------------------------------

**KeyWords:**

portName: string

port: int (0~5)

color: string (none/red/green/blue/yellow)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetColorRes",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "color": "black"
 }

}
```
