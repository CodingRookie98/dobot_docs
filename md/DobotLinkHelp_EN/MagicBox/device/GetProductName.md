# 5.2.8 GetProductName

Get product name

(other devices need to be extended to use this interface)
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
    "method": "dobotlink.MagicBox.GetProductName",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json

```json
 {     "id": 1,     "jsonrpc": "2.0",     "result": {      "productName": "Magician"
     }   
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com