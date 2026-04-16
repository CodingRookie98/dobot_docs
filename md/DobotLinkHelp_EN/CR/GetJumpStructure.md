# 7.25.10 GetJumpStructure

功能:

获取jump速度参数 



 INPUT: 

```json

{
    "id": 1,
     "jsonrpc": "2.0",
      "method": "dobotlink.CR.GetJumpStructure",

    "params": 
{         "portName": "192.168.5.1"    }}


```

OUTPUT：

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {"motors":[{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":false,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true},{"composite":false,"encoder":{"bitNum":14.2877123795,"type":""},"gearBox":{"den":101,"num":1},"motor":{"inverted":true,"limit":3500,"rated":3000,"type":""},"positionScaling":{"den":1,"num":360},"simulated":true}],"structure":{"L1":147,"L2":0,"L3":0,"L4":143.028,"L5":119.9334,"L6":104.5,"L7":0,"a1":0,"a2":-427.3999,"a3":-356.1736,"a4":0,"a5":0,"a6":0,"armSingularity12":100,"elbowSingularity12":10,"inclinationAngle":0.66,"limits":[[-178,178],[-178,178],[-160,160],[-178,178],[-178,178],[-357,357]],"rotationAngle":0.55,"wristSingularity12":10}}}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)