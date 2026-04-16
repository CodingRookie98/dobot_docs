# 9.8.2 SetStopPointParam

Set automatic parking service parameters 



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| scopeErr | int | yes | enter the parking range, the default 
      parameter is 40cm |
| stopErr | int | yes | parking accuracy, default parameter 
  2cm |







response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |







KeyWords:

portName: string

scopeErr: int, enter the parking range, the default parameter is 40cm

stopErr: int, parking accuracy, default parameter 2cm



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetStopPointParam",
    "params": {
        "portName": "COM4",
        "scopeErr": 40,
        "stopErr" : 2
    }
}
```

OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)