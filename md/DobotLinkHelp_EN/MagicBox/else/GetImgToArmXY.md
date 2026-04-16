# 9.8.4 GetImgToArmXY

Image coordinate to manipulator coordinate



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| imgX | float | yes | image coordinate X |
| imgY | float | yes | image coordinate y |
| needTranxy | int | yes | need to convert XY |
| suckApriltag | int | yes | grab QR code |
| apriltagHeight | int | yes | grab QR code 
height |







response result


| field | type | required | explain |
| --- | --- | --- | --- |
| armX | float | yes | manipulator coordinate X |
| armY | float | yes | manipulator coordinate Y |
| okflag | int | yes | whether the operation is successful (1: 
      success, others: failure) |







KeyWords:

portName: string

imgX: float, image coordinate x 

imgY: float, image coordinate y

needTranxy: int, need to convert xy 

suckApriltag: int,grab QR code 

apriltagHeight: int,grab QR code height 



INPUT:

```json

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

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "armX": 263.8121643066406,        "armY": -64.5769271850586,        "okflag": 1    }}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com