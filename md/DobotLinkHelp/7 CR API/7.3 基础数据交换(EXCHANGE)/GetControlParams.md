### 7.3.26 GetControlParams

功能:

获取exchange接口中的 controlParams 字段

INPUT:

```json
{

 "id": 1,

 "jsonrpc": "2.0",

 "method": "dobotlink.CR.GetControlParams",

 "params": {

 "portName": "192.168.5.1"

 }
}

```

OUTPUT：

```json
{
 "id": 1,

 "jsonrpc": "2.0",

 "result": [0, 1, 2, 3] //0温度，1电压，2功率，3电流
}
```
