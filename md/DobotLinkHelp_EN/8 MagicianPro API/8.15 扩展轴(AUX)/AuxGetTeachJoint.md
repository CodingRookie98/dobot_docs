**Description: 获取扩展轴示教参数**

**KeyWords:**

portName: string

velocity: List\<float\>

acceleration : List\<float\>

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxGetTeachJoint",
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
        "velocity": [100.0, 100.0, 100.0,100.0], 
        "acceleration": [100.0, 100.0, 100.0,100.0]
    }
}
```