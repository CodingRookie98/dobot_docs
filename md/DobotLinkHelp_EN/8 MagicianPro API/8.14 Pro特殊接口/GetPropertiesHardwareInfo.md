**Description: 获取设备硬件信息**

**KeyWords:**

portName: string

data: object

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetPropertiesHardwareInfo",
    "params": {
        "portName": "192.168.1.6" 
    }
}
```

 

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "SNcode" : "NULL",              //序列号
        "ControllerVersion" : "NULL",   //控制器硬件版本号
        "ServoVersion":"NULL"
    }
}
```