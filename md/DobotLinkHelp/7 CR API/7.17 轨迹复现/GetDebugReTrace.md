### 7.17.3 GetDebugReTrace

**功能: 轨迹复现获取**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetDebugReTrace",
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
    "result": {
        "currentTimes" : xx   //复现次数
        "isDone":"true/false" //复现完成
    }
}
```
