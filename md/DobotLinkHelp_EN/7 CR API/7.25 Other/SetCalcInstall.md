功能:

    获取安装姿态,平板发送当前笛卡尔点数据，控制器返回安装角度  

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",

    "method": "dobotlink.CR.SetCalcInstall",

    "params": {

        "portName": "192.168.5.1",

   "data":{"cartesianCoord":[x,y,z,a,b,c]}

      }


 
} 
  

```

OUTPUT：

``` language-json
  
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
  "SlopeAngle": 0.0,
  "RotationAngle": 0.0
 }
}
```