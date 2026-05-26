**Description: 获取电池电压**

**KeyWords:**

portName: string

PowerVoltage: float （电池电压）

PowerPercentage: float （电量）

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetBatteryVoltage",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "powerVoltage": 50.1, //电池电压
        "powerPercentage": 0.5 //电量
    }
}
```
