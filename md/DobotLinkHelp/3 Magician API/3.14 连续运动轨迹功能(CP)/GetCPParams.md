### 3.14.2 GetCPParams

**KeyWords:**

portName: string

targetAcc: float

junctionVel: float

isRealTimeTrack: bool

*acc: float (isRealTimeTrack = false)

*period: float (isRealTimeTrack = true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.GetCPParams",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": false,
        "acc": 100
    }
}
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "portName": "COM4",
        "targetAcc": 200,
        "junctionVel": 100,
        "isRealTimeTrack": true,
        "period": 20
    }
}
```
