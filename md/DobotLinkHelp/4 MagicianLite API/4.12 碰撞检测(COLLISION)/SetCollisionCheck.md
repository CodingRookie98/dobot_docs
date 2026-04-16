### 4.12.1 SetCollisionCheck

**设置碰撞检测功能**

请求参数 params

  ------------ --------- ------------ --------------------------------------------------
  字段        类型    是否必填   说明
  portName    string   是          通信端口
  enable      bool     是          是否开启碰撞功能（false：否，true：是）
  threshold   float    是          碰撞检测触发的角度阈值，单位° （取值范围：8-15）
  ------------ --------- ------------ --------------------------------------------------

响应参数 result

  --------- ------- ----------- ----------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true：操作成功，false：操作失败）
  --------- ------- ----------- ----------------------------------------------

**KeyWords:**

portName: string

enable: bool

threshold: float (min:8 unit:angle)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCollisionCheck",
    "params": {
        "portName": "COM4",
        "enable": true,
        "threshold": 9.5
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
