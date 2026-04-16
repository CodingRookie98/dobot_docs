# 9.8.3 GetStopPointState

Query whether the automatic parking service has stopped 



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |





KeyWords:

portName: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetStopPointState",
    "params": {
        "portName": "COM4" 
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "result": true    }}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)