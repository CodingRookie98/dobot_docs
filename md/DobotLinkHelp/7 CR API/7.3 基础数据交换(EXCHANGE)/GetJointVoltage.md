### 7.3.28 GetJointVoltage

功能:

获取exchange接口中的 jointVoltage 字段

INPUT:

```json
{

  "id": 1,

  "jsonrpc": "2.0",

 "method": "dobotlink.CR.GetJointVoltage",

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

 "result": [j1, j2, j3, j4, j5, j6]

}
```
