**Description: 获取扩展轴开关状态**

**KeyWords:**

portName: string

auxJoint: bool，轴功能开关

addPoints: bool，示教点功能开关

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxGetSwitch",
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
        "auxJoint": true,
        "addPoints": true
    }
}
```