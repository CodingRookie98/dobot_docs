# 5.11.2 SetBleInf

Set Bluetooth master-slave mode


request params






| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| mode | int | yes | master slave mode (0-master mode, 1-slave 
      mode) |
| name | string | yes | string, the length is within 
      14 bytes, and the insufficient part is filled with 
  0 |





响应参数 result

| 字段 | 类型 | 是否必填 | 说明 |
| --- | --- | --- | --- |
| result | bool | 是 | response result (true: operation succeeded, 
      false: operation failed) |








KeyWords:

portName: string

mode: int, 0-主机模式，1-从机模式

name: string, 长度在14字节以内



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetBleInf",
    "params": {
        "portName": "COM4",
        "mode": 1,
        "name": "string"
    }
}
```



OUTPUT：

```json

```json

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com