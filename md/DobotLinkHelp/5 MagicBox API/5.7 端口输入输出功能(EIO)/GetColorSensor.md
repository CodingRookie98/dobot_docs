### 5.7.12 GetColorSensor

**读取颜色传感器**

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

响应参数 result

  -------- ------- ----------- -----------
  字段    类型   是否必填   说明
  blue    int    是         蓝色阈值
  green   int    是         绿色阈值
  red     int    是         红色阈值
  -------- ------- ----------- -----------

**KeyWords:**

portName: string

red: int

green: int

blue: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetColorSensor",
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

 "blue": 0,
 "green": 0,
 "red": 0

 }

}
```
