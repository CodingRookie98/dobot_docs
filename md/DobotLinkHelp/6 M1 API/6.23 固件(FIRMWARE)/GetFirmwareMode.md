### 6.23.5 GetFirmwareMode

**KeyWords:**

portName: string

firmwareMode: int(0:INVALID_MODE 1:DOBOT_MODE 2:PRINTING_MODE
3:OFFLINE_MODE 4:MTEST_MODE 5:BROKEN_MODE)

ctrl: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetFirmwareMode",
    "params": {
        "portName": "COM4"
    }
}
```
