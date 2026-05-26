**Description: 获取IMU加速度值与角速度值**

**KeyWords:**

portName: string

ax: float(加速度，g)

ay: float(加速度，g)

az: float(加速度，g)

gx: float(角速度，°/s)

gy: float(角速度，°/s)

gz: float(角速度，°/s)

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.GetImuSpeed",
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
              "ax": 10.0,
         "ay": 10.0,
         "az": 10.0,
         "gx": 10.0,
         "gy": 10.0,
         "gz": 10.0
     }
}
```
