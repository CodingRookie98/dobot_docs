# 4.2.8 GetProductName

Get device name
request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |

response result
| field | type | required | explain |
| --- | --- | --- | --- |
| productName | string | yes | product 
name |


KeyWords:

portName: string

productName: string



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetProductName",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:

```json

```json
 {     "id": 1,     "jsonrpc": "2.0",     "result": {         "productName": "Magician"     }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com