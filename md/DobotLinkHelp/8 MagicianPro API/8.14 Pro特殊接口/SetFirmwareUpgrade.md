### 8.14.17 SetFirmwareUpgrade

**Description: 固件升级**

**KeyWords:**

portName: string

type: string

index: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetFirmwareUpgrade",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "type" : "xml"/"foe",
            "index" : 1    //1.伺服
        }
    }
}
```
