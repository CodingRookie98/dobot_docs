## 2.13 SwitchLanguage

**Description: 切换dobotlink的语言**

**KeyWords:**

language: string ("en"英文, "ch"中文)

!!! 注意: 切换成英文时需要调用两遍该接口...

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.api.SwitchLanguage",
    "params": {
        "language": "en"/"ch"
    }
}
```
