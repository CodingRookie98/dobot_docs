**Description: 设置脚本的启动与退出**

**KeyWords:**

portName: string

isEnable: int (0:STOP 1:START)

name: String

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetMagicBoxScriptMode",
    "params": {
        "portName": "COM4",
        "isEnable": 1 ,//1启动脚本，0退出脚本（不需要脚本名）
        "name": Playback/***.py或Script/***.py或Draw/***.py
    }
}
```