### 7.7.2 SetCalibrateToolPosition

**功能: CR工具坐标系位置标定**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetCalibrateToolPosition",
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

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "result": true,
        "coordinate": [X, Y, Z],
        "deviation": 0.001
    }
}
```
