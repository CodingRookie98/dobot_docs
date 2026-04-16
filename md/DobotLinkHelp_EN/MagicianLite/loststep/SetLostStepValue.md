# 4.11.1 SetLostStepValue

Set step loss detection function

request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| value | float | yes | step loss detection deviation value (value range: 
  8-15) |





response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation 
      succeeded, false: operation failed) |








KeyWords:

portName: string

value: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetLostStepValue",
    "params": {
        "portName": "COM4",
        "value": 10
    }
}
```



OUTPUT:

```json

```json
{    "id": 1,     "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com