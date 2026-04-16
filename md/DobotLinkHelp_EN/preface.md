# 1 matters needing attention

Brief introduction



 DobotLink is an intermediate service layer for the communication between hardware equipment and host computer (DobotLab or other development environment). All external software control Dobot's hardware equipment through this service layer, including magician, magician lite, magician Go, etc. DobotLink not only includes API dynamic library, but also supports firmware update, device verification and other functions of equipment.



Protocol description





 This protocol describes the data format in which the client interacts with DobotLink. DobotLink sends instructions to the device through the interface, and the device returns the response result after running the instructions.


DobotLink, as the server, uses websocket communication, and the listening port is 9090Data interaction protocol conforms to jsonrpc2 0 transport protocol DobotLink applicable system version: win7 / win10Instruction type requirements: queue instructions (some instructions can be modified to immediate instructions through the isqueued field)
The agreement is as follows:

request data


| field | type | required | explain |
| --- | --- | --- | --- |
| id | long | yes | identification of the request; in each 
      request, the value should not be the same as far as possible, and the 
      server must return with the same ID |
| jsonrpc | string | yes | indicates the protocol version. fill in the 
      fixed value: 2.0 |
| method | string | yes | request interface |
| params | object | no | request parameters; depending on the 
      method, if there is no parameter, it can not be 
passed |



response data


| field | type | required | explain |
| --- | --- | --- | --- |
| id | long | yes | identification of response; must be the 
      same as the ID at the time of the request |
| jsonrpc | string | yes | indicates the protocol version. fill in the 
      fixed value: 2.0 |
| result | object | yes | response return data; it varies according 
      to the request interface. If you do not need to return results, this field 
      must be filled in 
    null |








Note: in the later chapters of this document, the meanings of ID, jsonrpc and method will not be explained again. Only the parameters and result fields will be introduced in detail.












 Example： 

Get red and blue button sensor status

Request  {  "id": 1, "jsonrpc": "2.0",  "method": "dobotlink.MagicBox.GetButtonStatus", "params": {  "port": 0,  "portName": "COM4"  } }

Response {  "id": 1,  "jsonrpc": "2.0",  "result": {  "blueBtn": 1, "redBtn": 1  }  }

matters needing attention



DobotLink needs to be installed to connect and use Dobot hardware devices

Each host computer has and can only run one dobotlink

The port (1-6) of the device corresponds to the port number (0-5) of the interface document

Document revision description






































| serial 
      number | time | version | revision 
      description | reviser | remark |
| --- | --- | --- | --- | --- | --- |
| 1 | 2019.11.11 | V1.0.0 | create 
      documents | liuyufei |  |
| 2 | 2021.12.07 | V5.43 | modify document | Kenan Wu |  |








Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com