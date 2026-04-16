### 8.14.14 SetPropertiesHardwareInfo

**Description: 设备硬件信息**

**KeyWords:**

portName: string

data: object

SNcode: string

ControllerVersion: string

ServoVersion: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetPropertiesHardwareInfo",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "SNcode" : "NULL",              //序列号
            "ControllerVersion" : "NULL",   //控制器硬件版本号
            "ServoVersion":"NULL"           //伺服硬件版本号
        }
    }
}
```
