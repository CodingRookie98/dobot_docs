### 4.12.2 GetCollisionCheck

**读取碰撞检测功能**

请求参数 params

  ----------- --------- ------------ -----------
  字段       类型    是否必填   说明
  portName   string   是          通信端口
  ----------- --------- ------------ -----------

<div>

响应参数 result

</div>

<div>

</div>

<div>

</div>

  ------------ -------- ----------- ------------------------------------------
  字段        类型    是否必填   说明
  isEnabled   bool    是         是否开启碰撞功能（false：否，true：是）
  threshold   float   是         碰撞检测触发的角度阈值，单位°
  ------------ -------- ----------- ------------------------------------------

**KeyWords:**

portName: string

isEnabled: bool

threshold: float

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetCollisionCheck",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "isEnabled": true,
 "threshold": 8
 }

}
```
