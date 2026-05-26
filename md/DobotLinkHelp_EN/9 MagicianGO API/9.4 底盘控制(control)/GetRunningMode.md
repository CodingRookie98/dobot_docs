**Description: 获取运行模式**

**KeyWords:**

portName: string

runningState: int (0:NORMAL MODE 1:SAFE MODE)

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetRunningMode",
    "params": {
        "portName": "COM4",
    }
}
```