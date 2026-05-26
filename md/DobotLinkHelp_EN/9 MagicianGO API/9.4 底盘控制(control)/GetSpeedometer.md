**Description: 获取里程计数据**

**KeyWords:**

portName: string

x: float(m)

y: float(m)

yam: float(°)

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetSpeedometer",
    "params": {
        "portName": "COM4"
    }
}
```