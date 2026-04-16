# 9.4.16 SetBuzzerSound

Description: 设置蜂鸣器音效 

KeyWords:

portName: string

index: int （音乐索引）0：关闭， 1：鸣叫， 2：定时关闭， 3：滴， 4：滴滴滴， 5：滴~滴滴， 6：滴滴滴滴滴 12345 (1234567代表音调dou ruai mi fa so la xi)， 7：鸣笛提示音：1414 

tone: int （音调）（index 0-2有效）(取值范围0-84但低数字区域声音模拟的不好，测试建议选用中间部分如50)

beat: float （节拍）（index 2有效，单位秒）



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetBuzzerSound",
    "params": {
        "portName": "COM4",
        "index": 1,
        "tone": 1,
        "beat": 1
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)