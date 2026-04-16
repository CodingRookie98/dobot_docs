### 4.2.8 GetProductName

[获取产品名称]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

</div>

<div>

[请求参数
params]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

</div>

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

</div>

<div>

[
]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

  ----------- --------- ----------- ----------
  字段       类型     是否必填   说明
  portName   string   是         通信端口
  ----------- --------- ----------- ----------

</div>

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

</div>

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

</div>

<div>

[
]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

<div>

响应参数 result

</div>

<div>

</div>

<div>

  -------------- -------- ----------- ----------
  字段          类型    是否必填   说明
  productName   string   是         产品名称
  -------------- -------- ----------- ----------

</div>

</div>

<div>

[]{style="FONT-SIZE: 10.45pt; FONT-FAMILY: 宋体; FONT-WEIGHT: bold; COLOR: rgb(0,176,80); mso-spacerun: 'yes'"}

</div>

**KeyWords:**

portName: string

productName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetProductName",
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
 "productName": "Magician"
 }

}
```
