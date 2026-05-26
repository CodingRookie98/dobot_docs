设置传感器角度系数，用于自动调平接口

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Magician.SetAngleSensorCoef",

    "params": {

        "portName": "192.168.5.1",

       "rearArmAngle": 0.97,

        "frontArmAngle": 0.98

    }
}
```

OUTPUT：

``` language-json
{
    "id": 1,

    "jsonrpc": "2.0",

    "result": true
}
```
