**Description: 返回控制器报警信息文件**

**KeyWords:**

portName: string

data: object

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetAlarmController",
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
        [
    {
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
        "id": 16,
        "level": 0,
        "en": {
            "description" : "Inverse kinematics error with singularity",
            "cause" : "",
            "solution" : ""
        },
        "zh_CN": {
            "description" : "逆解算奇异",
            "cause" : "",
            "solution" : ""
        }
    },... ...]
    }
}
```