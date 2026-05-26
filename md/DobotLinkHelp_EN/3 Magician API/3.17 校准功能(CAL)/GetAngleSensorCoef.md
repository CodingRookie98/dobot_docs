获取传感器角度系数，用于自动调平接口

INPUT:

``` language-json
{   
    "id": 1,    

    "jsonrpc": "2.0",    

    "method": "dobotlink.Magician.GetAngleSensorCoef",

    "params": {       

         "portName": "192.168.5.1"

      }


}
```

OUTPUT：

``` language-json
{    
    "id": 1,    
    "jsonrpc": "2.0",
    "result":{        
        "rearArmAngle": 0.9707000255584717,
        "frontArmAngle":0.9922999739646912

    }
}
```