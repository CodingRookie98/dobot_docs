**Description: 设置扩展轴再现参数**

**KeyWords:**

portName: string

velocity: List\<float\>

acceleration: List\<float\>

jerk: List\<float\>

INPUT:

``` language-json

{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxSetPlaybackJoint",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "velocity": [100.0, 100.0, 100.0, 100.0],
            "acceleration": [100.0, 100.0, 100.0, 100.0],
            "jerk": [100.0, 100.0, 100.0, 100.0]
        }    
    }
}
```