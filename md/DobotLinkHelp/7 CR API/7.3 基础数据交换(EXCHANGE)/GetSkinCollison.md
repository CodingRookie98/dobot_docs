### 7.3.24 GetSkinCollison

功能:

获取exchange接口中的 skinCollison 字段

INPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "method": "dobotlink.CR.GetSkinCollison",
 "params": {
 "portName": "192.168.5.1"
 }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": 1/0 //1 发生电子皮肤碰撞, 0 未发生电子皮肤碰撞
}
```
