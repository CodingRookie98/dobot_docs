### 5.3.7 GetQueuedCmdLeftSpace

<div>

[**获取指令队列剩余空间**]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; COLOR: rgb(0,0,0); mso-spacerun: 'yes'"}

</div>

请求参数 params

  ----------- --------- ----------- -----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- -----------

<div>

响应参数 result

</div>

<div>

</div>

<div>

</div>

<div>

  ------------ ------- ----------- --------------
  字段        类型   是否必填   说明
  leftSpace   int     是         剩余空间数量
  ------------ ------- ----------- --------------

</div>

**KeyWords:**

portName: string

leftSpace: int

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetQueuedCmdLeftSpace",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "leftSpace": 32
 }

}
```
