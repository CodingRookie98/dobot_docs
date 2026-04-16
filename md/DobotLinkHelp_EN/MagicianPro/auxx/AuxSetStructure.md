# 8.15.8 AuxSetStructure

Description: 设置扩展轴其他参数

KeyWords:

portName: string





 INPUT:

```json
 
 
```json

{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxSetStructure",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "auxJoint":3, //扩展轴数量
            "type":[0,0,0], //0-关节，1-直线
            "limits":
            [
                [0, 0],--范围限制
                [0, 0],
                [0, 0]
            ],
            "motors": [
                {
                    "composite": false,
                    "encoder": {
                        "bitNum": 17,--编码器位数
                        "type": ""
                    },
                    "gearBox": {
                        "den": 50, --减速比分母
                        "num": 1 --减速比分子
                    },
                    "motor": {
                        "inverted": false, --电机转动方向
                        "limit": 5500, --最大转速
                        "rated": 5000, --额定转速
                        "type": ""
                    },
                    "positionScaling": {
                        "den": 1,
                        "num": 360
                    },
                    "simulated": true --虚/实轴
                },
                {
                    "composite": false,
                    "encoder": {
                        "bitNum": 17,
                        "type": ""
                    },
                    "gearBox": {
                        "den": 50,
                        "num": 1
                    },
                    "motor": {
                        "inverted": false,
                        "limit": 5500,
                        "rated": 5000,
                        "type": ""
                    },
                    "positionScaling": {
                        "den": 1,
                        "num": 360
                    },
                    "simulated": true
                },
                {
                    "composite": false,
                    "encoder": {
                        "bitNum": 17,
                        "type": ""
                    },
                    "gearBox": {
                        "den": 50,
                        "num": 1
                    },
                    "motor": {
                        "inverted": false,
                        "limit": 5500,
                        "rated": 5000,
                        "type": ""
                    },
                    "positionScaling": {
                        "den": 1,
                        "num": 360
                    },
                    "simulated": true
                }
            ]
        }
        
    }
}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)