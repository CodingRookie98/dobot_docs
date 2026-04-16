### 6.3.4 QueuedCmdStartDownload

**KeyWords:**

portName: string

totalLoop: int

linePerLoop: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.QueuedCmdStartDownload",
    "params": {
        "portName": "COM4"
        "totalLoop": 10,
        "linePerLoop": 20
    }
}
```
