### 5.1.3 DisconnectDobot

**断开设备连接**

<div>

请求参数 params

</div>

<div>

</div>

<div>

</div>

<div>

  ------------- ---------- ------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  字段         类型     是否必填   说明
  portName     string   是         通信端口
  queueStop    bool      否          [停止队列，默认为true(true：开启[停止队列]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}操作，false：关闭停止队列操作)]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}
  queueClear   bool      否         [ 清除队列，默认为true(true：开启清除[队列 ]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}操作，false：关闭清除队列操作)]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-font-kerning: 1.0000pt"}
  ------------- ---------- ------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
</div>

<div>

</div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- ----------------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         设备的连接状态（true：连接成功，false：连接失败）
  --------- ------- ----------- ----------------------------------------------------

</div>

**KeyWords:**

portName: string

*queueStop: bool (default:true)

*queueClear: bool (default:true)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.DisconnectDobot",
    "params": {
        "portName": "COM4",
        "queueStop": true,
        "queueClear": true
    }
}
```

OUTPUT：

```json
 {
 "id": 56,
   "jsonrpc": "2.0",
 "result": true
}

```
