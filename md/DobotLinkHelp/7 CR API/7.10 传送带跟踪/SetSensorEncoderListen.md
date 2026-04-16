### 7.10.3 SetSensorEncoderListen

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetSensorEncoderListen",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "cmd" : "start/stop",
            "conveyor_index" : int,
            "DI_index" : int,
            "trigger_type" : int
        }
    }
}
```
