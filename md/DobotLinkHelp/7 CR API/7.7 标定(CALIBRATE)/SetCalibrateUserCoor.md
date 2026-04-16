### 7.7.4 SetCalibrateUserCoor

**功能: CR用户坐标系标定设置**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCalibrateUserCoor",
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
  "result" :true/false,
  "coordinate" : [X, Y, Z, A, B, C]
}
}
```
