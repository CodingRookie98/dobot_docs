### 9.8.4 GetImgToArmXY

**图像坐标转机械臂坐标**

请求参数 params

  ----------------- --------- ----------- -----------------
  字段             类型     是否必填   说明
  portName         string   是         通信端口
  imgX             float    是         图像坐标X
  imgY             float    是         图像坐标Y
  needTranxy       int      是         是否需要转换XY
  suckApriltag     int      是         抓取二维码
  apriltagHeight   int      是         抓取二维码高度
  ----------------- --------- ----------- -----------------

响应参数 result

  --------- -------- ----------- --------------------------------------
  字段     类型    是否必填   说明
  armX     float   是         机械臂坐标X
  armY     float   是         机械臂坐标Y
  okflag   int     是         是否运行成功（1：成功，其它：失败）
  --------- -------- ----------- --------------------------------------

**KeyWords:**

portName: string

imgX: float, 图像坐标X

imgY: float, 图像坐标Y

needTranxy: int,是否需要转换XY

suckApriltag: int,抓取二维码

apriltagHeight: int,抓取二维码高度

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetImgToArmXY",
    "params": {
        "portName": "COM4",
        "imgX": 50.1,
        "imgY": 100.8,
        "needTranxy": 1,
        "suckApriltag": 1,
        "apriltagHeight":10
    }
}
```

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": {
 "armX": 263.8121643066406,
 "armY": -64.5769271850586,
 "okflag": 1
 }
}
```
