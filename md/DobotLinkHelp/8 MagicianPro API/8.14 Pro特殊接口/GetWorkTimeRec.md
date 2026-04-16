### 8.14.19 GetWorkTimeRec

**Description: 获取累计运行时间**

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetWorkTimeRec",
    "params": {
        "portName": "192.168.1.6"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "powerOnTime": {
              "days": 0000,
              "hour": 00,
              "min": 27,
              "sec": 02,
        },
        "enableTime": {
              "days": 0000,
              "hour": 00,
              "min": 00,
              "sec": 00,
        }
    }
}
```
