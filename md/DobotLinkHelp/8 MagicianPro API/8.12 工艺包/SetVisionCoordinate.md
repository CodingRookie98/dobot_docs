### 8.12.1 SetVisionCoordinate

**Description: 获取相机坐标**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetVisionCoordinate",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "ip" : "相机IP",
            "port":"相机Port",
            "index":"相机编号"
        }
    }
}
```
