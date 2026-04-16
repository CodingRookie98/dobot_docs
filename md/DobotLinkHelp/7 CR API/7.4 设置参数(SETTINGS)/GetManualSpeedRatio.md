### 7.4.20 GetManualSpeedRatio

**CR弃用**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetManualSpeedRatio",
    "params": {
        "portName": "192.168.5.1"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result":  [{
            "enable": true,
            "params": {
                "startHeight": 10,
                "endHeight": 15,
                "zLimit": 200
            }
        }, {
            "enable": false,
            "params": {
                "startHeight": 11,
                "endHeight": 20,
                "zLimit": 200
            }
    }]
}
```
