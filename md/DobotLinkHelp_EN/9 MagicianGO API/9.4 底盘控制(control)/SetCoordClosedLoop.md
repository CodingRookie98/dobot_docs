**Description: 设置世界坐标系下角度闭环**

**KeyWords:**

portName: string

isEnable: int (是否使能角度闭环)

angle: float (角度，°（-180-180）)

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetCoordClosedLoop",
    "params": {
        "portName": "COM4",
        "isEnable": 1 ,
        "angle":10
    }
}
```