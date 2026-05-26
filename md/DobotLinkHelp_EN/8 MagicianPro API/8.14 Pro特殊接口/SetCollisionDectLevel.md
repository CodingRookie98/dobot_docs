**Description: 设置安全碰撞等级**

**KeyWords:**

portName: string

data: object

Level: int (等级设置1~5)

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetCollisionDetectLevel",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            'Level': 1
        }
    }
}
```