### 5.10.1 DownloadProgram

**下载离线脚本到Box的U盘中**

请求参数 params

  ----------- --------- ----------- -----------------------------------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  code       string   是         base64转码utf8编码格式的文件内容
  fileName   string   是         文件名
  ----------- --------- ----------- -----------------------------------

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

**KeyWords:**

portName: string

code: string，base64转码utf8编码格式的文件内容

*fileName: string (default:temp)，文件名

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.DownloadProgram",
    "params": {
        "portName": "COM4",
        "code": "# -*- coding: UTF-8 -*-n ...... ",
        "fileName": "dobot_scratch.py"
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
