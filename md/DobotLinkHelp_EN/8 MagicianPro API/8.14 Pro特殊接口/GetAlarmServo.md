**Description: 返回伺服报警信息文件**

**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetAlarmServo",
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
        [{
        "id": 0,
        "level": 0,
        "en": {
            "description" : "No error",
            "cause" : "",
            "solution" : ""
        },
        "zh_CN": {
            "description" : "无错误",
            "cause" : "",
            "solution" : ""
        }
        },
        {
        "id": 1,
        "level": 0,
        "en": {
            "description" : "Communication error",
            "cause" : "",
            "solution" : ""
        },
        "zh_CN": {
            "description" : "通讯错误",
            "cause" : "",
            "solution" : ""
        }
        },... ...]
    }
}
```
