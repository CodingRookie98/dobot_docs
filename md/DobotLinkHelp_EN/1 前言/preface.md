**Brief introduction**

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"></span> 

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"> 
DobotLink is an intermediate service layer for the communication between
hardware equipment and host computer (DobotLab or other development
environment). All external software control Dobot\'s hardware equipment
through this service layer, including magician, magician lite, magician
Go, etc. DobotLink not only includes API dynamic library, but also
supports firmware update, device verification and other functions of
equipment.</span>

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"></span> 

**Protocol description**

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"></span>

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"></span> 

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt">
This protocol describes the data format in which the client interacts
with DobotLink. DobotLink sends instructions to the device through the
interface, and the device returns the response result after running the
instructions.</span>

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"></span> 

DobotLink, as the server, uses websocket communication, and the
listening port is 9090

Data interaction protocol conforms to jsonrpc2 0 transport protocol

DobotLink applicable system version: win7 / win10

Instruction type requirements: queue instructions (some instructions can
be modified to immediate instructions through the isqueued field)

**The agreement is as follows:**

request data

|          |         |          |                                                                                                                                                   |
|----------|---------|----------|---------------------------------------------------------------------------------------------------------------------------------------------------|
|  field   |  type   | required | explain                                                                                                                                           |
|  id      |  long   |  yes     |  identification of the request; in each request, the value should not be the same as far as possible, and the server must return with the same ID |
|  jsonrpc |  string |  yes     |  indicates the protocol version. fill in the fixed value: 2.0                                                                                     |
|  method  |  string |  yes     |  request interface                                                                                                                                |
|  params  |  object |  no      |  request parameters; depending on the method, if there is no parameter, it can not be passed                                                      |

response data

|          |         |           |                                                                                                                                              |
|----------|---------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
|  field   |  type   |  required |  explain                                                                                                                                     |
|  id      |  long   |  yes      |  identification of response; must be the same as the ID at the time of the request                                                           |
|  jsonrpc |  string |  yes      |  indicates the protocol version. fill in the fixed value: 2.0                                                                                |
|  result  |  object |  yes      |  response return data; it varies according to the request interface. If you do not need to return results, this field must be filled in null |

-   Note: in the later chapters of this document, the meanings of ID,
    jsonrpc and method will not be explained again. Only the parameters
    and result fields will be introduced in detail.

**Example：**

Get red and blue button sensor status

Request   
{  
    \"id\": 1,  
    \"jsonrpc\": \"2.0\",  
    \"method\": \"dobotlink.MagicBox.GetButtonStatus\",  
    \"params\": {  
        \"port\": 0,  
        \"portName\": \"COM4\"  
    }  
}

Response  
{  
    \"id\": 1,  
    \"jsonrpc\": \"2.0\",  
    \"result\": {  
        \"blueBtn\": 1,  
        \"redBtn\": 1  
    }  
}

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
**matters needing attention**</span>

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
</span> 

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
DobotLink needs to be installed to connect and use Dobot hardware
devices</span>

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
Each host computer has and can only run one dobotlink</span>

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
</span>

The port (1-6) of the device corresponds to the port number (0-5) of the
interface document

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
</span>

**Document revision description**

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
</span>

 

<table class="MsoTableGrid"
style="BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 426pt; BORDER-COLLAPSE: collapse; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; mso-table-layout-alt: fixed; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext; mso-border-insideh: 0.5000pt solid windowtext; mso-border-insidev: 0.5000pt solid windowtext; mso-padding-alt: 0.0000pt 5.4000pt 0.0000pt 5.4000pt"
data-cellspacing="0" data-border="1">
<colgroup>
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
</colgroup>
<tbody>
<tr class="odd">
<td
style="BORDER-TOP: windowtext 1pt solid; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">serial
number</span> <span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: windowtext 1pt solid; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">time</span><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: windowtext 1pt solid; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">version</span></p></td>
<td
style="BORDER-TOP: windowtext 1pt solid; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">revision
description</span></p></td>
<td
style="BORDER-TOP: windowtext 1pt solid; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">reviser</span><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: windowtext 1pt solid; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">remark</span></p></td>
</tr>
<tr class="even" style="HEIGHT: 16pt">
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">1</span><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">2019.11.11</span><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">V1.0.0</span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">create
documents</span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">liuyufei
</span><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
</tr>
<tr class="odd">
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">2</span><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"></span></p>
<p>2021.12.07 </p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">
</span>
<p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt">V5.43</span></p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p>
<p> modify document</p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"></span></p>
<p>Kenan Wu</p></td>
<td
style="BORDER-TOP: #f0f0f0; BORDER-RIGHT: windowtext 1pt solid; WIDTH: 71pt; BORDER-BOTTOM: windowtext 1pt solid; PADDING-BOTTOM: 0pt; PADDING-TOP: 0pt; PADDING-LEFT: 5.4pt; BORDER-LEFT: windowtext 1pt solid; PADDING-RIGHT: 5.4pt; BACKGROUND-COLOR: transparent; mso-border-left-alt: 0.5000pt solid windowtext; mso-border-top-alt: 0.5000pt solid windowtext; mso-border-right-alt: 0.5000pt solid windowtext; mso-border-bottom-alt: 0.5000pt solid windowtext"
data-valign="top" width="94"><p><span
style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-fareast-font-family: 宋体; mso-bidi-font-family: &#39;Times New Roman&#39;; mso-font-kerning: 1.0000pt"></span></p></td>
</tr>
</tbody>
</table>

 

 

<span style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri">
</span>