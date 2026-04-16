### 5.9.1 SetUpgradeStatus

**设置固件烧录状态**

请求参数 params

  ----------- --------- ----------- ----------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  length     string   是         固件长度（4字节）
  md5        string   是         md5校验码（16字节）
  ----------- --------- ----------- ----------------------

<div>

</div>

<div>

响应参数 result

</div>

<div>

</div>

<div>

  --------- ------- ----------- --------------------------------------------
  字段     类型   是否必填   说明
  result   bool    是         响应结果（true:操作成功，false:操作失败）
  --------- ------- ----------- --------------------------------------------

</div>

**Description: 将设备切换成固件烧录的模式**

**KeyWords:**

portName: string

length: string

md5: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetUpgradeStatus",
    "params": {
        "portName": "COM4",
        "length": "B0060800",
        "md5": "6094308AA9DED6A612A620AC4A195615"
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
