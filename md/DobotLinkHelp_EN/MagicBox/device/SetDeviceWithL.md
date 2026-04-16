# 5.2.5 SetDeviceWithL

Set equipment slide status


request params








| field | type | required | explain |
| --- | --- | --- | --- |
| enable | bool | yes | enable the slide rail. True: enable; False: not 
      enabled |
| version | int | yes | slide rail version number (0: V1 version, 1: V2 
      version) |




response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: setting succeeded, 
      false: setting failed) |




KeyWords:

portName: string

enable: bool

version: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetDeviceWithL",
    "params": {
        "portName": "COM4",
        "enable": true,
        "version": 1
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true    
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com