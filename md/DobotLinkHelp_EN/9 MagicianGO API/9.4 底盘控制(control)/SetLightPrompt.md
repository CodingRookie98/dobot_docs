**Description: 设置提示灯光**

**KeyWords:**

portName: string

index: int (0：空闲 1：USB 2：蓝牙提示 3：手柄 4：脚本 )

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetLightPrompt",
    "params": {
        "portName": "COM4",
        "index": 0
    }
}
```
