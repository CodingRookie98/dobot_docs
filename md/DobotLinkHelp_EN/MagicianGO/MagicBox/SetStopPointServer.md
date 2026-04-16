# 9.8.1 SetStopPointServer

Start the automatic parking service and pass in a point. When the vehicle reaches the point, it will stop automatically



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| PointX | int | yes | X coordinate of parking point |
| PointY | int | yes | Y coordinate of parking 
point |







 response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |











KeyWords:

portName: string

PointX: int， X coordinate of parking point

PointY: int，Y coordinate of parking point



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetStopPointServer",
    "params": {
        "portName": "COM4",
        "PointX" : 10,
        "PointY" : 10
    }
}
```

OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": true}

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)