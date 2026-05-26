**Description: 设置底盘在世界坐标系下移动到一点，根据目标点，速度移动**

**KeyWords:**

portName: string

x: （目标点x坐标）float(cm)

y: （目标点y坐标）float(cm)

s: （速度）float(0-100)cm/s

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetMovePos",
    "params": {
        "portName": "COM4",
        "x": 10.0,
        "y": 10.0,
        "s": 10.0,
    }
}
```