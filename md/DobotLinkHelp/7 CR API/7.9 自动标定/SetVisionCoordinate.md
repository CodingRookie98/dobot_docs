### 7.9.1 SetVisionCoordinate

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetVisionCoordinate",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "ip" : "相机IP",
            "port":"相机Port",
            "index":"相机编号"
        }
    }
}
```
