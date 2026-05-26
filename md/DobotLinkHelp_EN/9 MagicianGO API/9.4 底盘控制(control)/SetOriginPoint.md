**Description: 设置小车起点使能**

**KeyWords:**

portName: string

enable: int

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetOriginPoint",
    "params": {
        "portName": "COM4",
        "enable": 1 //1：使能 0：不使能
    }
}
```