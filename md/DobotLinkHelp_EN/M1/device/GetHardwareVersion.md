# 6.2.6 GetHardwareVersion

KeyWords:

portName: string

brakeBoard: string

driverFrontArm: string

driverRArm: string

driverRearArm: string

driverZArm: string

encoderFrontArm: string

encoderRArm: string

encoderRearArm: string

encoderZArm: string

endIOBoard: string

machineNum: string

mainBoard: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetHardwareVersion",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "brakeBoard":"PB105018AB",
        "driverFrontArm":"PB105001AC",
        "driverRArm":"PB105001AC",
        "driverRearArm":"PB105001AC",
        "driverZArm":"PB105001AC",
        "encoderFrontArm":"PB105002BC",
        "encoderRArm":"PB105002BC",
        "encoderRearArm":"PB105002BC",
        "encoderZArm":"PB105002BC",
        "endIOBoard":"PB105004BB",
        "machineNum":"0A000000000PB105006AD",
        "mainBoard":"PB105006AD"
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com