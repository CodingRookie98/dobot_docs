**Description: 开始监听传感器**

**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetSensorEncoderListen",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "cmd" : "start/stop",
            "conveyor_index" : int,
            "DI_index" : int,
            "trigger_type" : int
        }
    }
}
```
