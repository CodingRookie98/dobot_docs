INPUT:

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "method": "dobotlink.CR.SetHotkey",
 "params": {
 "portName": "192.168.5.1",
 "data": {
 "down": [17, 0, 18, 1],
 "downApi": "DO1_OFF_DO2_ON",
 "id": 3,
 "mode": 0,
 "name": "Terminal-IO",
 "up": [17, 0, 18, 0],

 "upApi": "DO1_OFF_DO2_OFF"

 }

 }

}
```
:::

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
