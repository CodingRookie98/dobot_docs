**Description: 设置安全碰撞恢复方式**

**KeyWords:**

portName: string

data: object

resumeType: int（0:正常恢复，1:等待5s自动恢复，2:外力恢复）

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetCollisionDetectResumeType",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            'resumeType': 1
        }
    }
}
```