### 7.7.3 SetCalibrateToolPose

**功能: CR工具坐标系姿态标定**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCalibrateToolPose",
    "params": {
        "portName": "192.168.5.1",
        "data": [
            [X, Y, Z, A, B, C],
            [X, Y, Z, A, B, C],
            [X, Y, Z, A, B, C]
        ]
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result":{
"result" : true/false,
"coordinate" : [X, Y, Z]
}
}
```
