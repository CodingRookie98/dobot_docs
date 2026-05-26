**MG400控制器版本1.4.6.0及以上后弃用**

 

**Description: 获取手动模式全局速度比例**

**KeyWords:**

portName: string

data: object

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetManualSpeedRatio",
    "params": {
        "portName": "192.168.1.6"
    }
}
```