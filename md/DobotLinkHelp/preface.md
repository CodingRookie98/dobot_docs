::: {#winchm_template_top}
::: {#winchm_template_button}
![Previous topic](template2/btn_prev_g.gif){#winchm_template_prev
border="0"}[![Next
topic](template2/btn_next_n.gif){#winchm_template_next
border="0"}](DobotLink/ShowCommMonitor.html "Next topic")
:::

::: {#winchm_template_navigation}
Help \>
:::

::: {#winchm_template_title}
1 DobotLink 开发协议说明
:::
:::

::: {#winchm_template_container}
::: {#winchm_template_content}
**简介**

[]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"} 

[ 
DobotLink是硬件设备与上位机（DobotLab或者其他开发环境）通信的中间服务层，所有外界软件都通过该服务层控制Dobot的硬件设备，包含magician、magician
lite、magician
Go等。DobotLink不仅包含API动态库，还支持设备的固件更新、设备校验等功能。]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"}

[]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"} 

 

[
**协议说明**]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"}

[]{style="FONT-SIZE: 
10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"} 

[
本协议说明了客户端与DobotLink交互的数据格式。DobotLink通过接口形式向设备发送指令，设备运行指令后返回响应结果。]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"}

[]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: Calibri; mso-spacerun: 'yes'; mso-fareast-font-family: 宋体; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt"} 

DobotLink作为服务端，采用Websocket通讯，监听端口为9090

数据交互协议符合 JsonRPC2.0传输协议

DobotLink适用系统版本：win7/win10   

指令类型要求：队列指令（部分指令可以通过isQueued字段修改成立即指令）

 

**协议如下：**

请求数据

  ---------- --------- ----------- ---------------------------------------------------------------------
   字段       类型      是否必填    说明
   id         long      是          请求的标识；每次请求时，该值尽量不要相同，服务端必须以相同的id返回
   jsonrpc    string    是          表示协议版本，填写固定值：2.0
   method     string    是          请求接口
   params     object    否          请求参数；根据method的不同而不同，如果没有参数，可以不传
  ---------- --------- ----------- ---------------------------------------------------------------------

响应数据

  ---------- --------- ----------- ----------------------------------------------------------------------------------
   字段       类型      是否必填    说明
   id         long      是          响应的标识；必须与请求时的id相同
   jsonrpc    string    是          表示协议版本，填写固定值：2.0
   result     object    是          响应返回数据；根据请求接口不同而不同，如果不需要返回结果，则该字段必须填写 null
  ---------- --------- ----------- ----------------------------------------------------------------------------------

-   <div>

    说明：本文档后面的章节中，不再重复讲解id,
    jsonrpc,method含义，只会针对params和result字段作具体介绍。

    </div>

**例子：**

获取红蓝按钮传感器状态

请求\
{\
    \"id\": 1,\
    \"jsonrpc\": \"2.0\",\
    \"method\": \"dobotlink.MagicBox.GetButtonStatus\",\
    \"params\": {\
        \"port\": 0,\
        \"portName\": \"COM4\"\
    }\
}

响应\
{\
    \"id\": 1,\
    \"jsonrpc\": \"2.0\",\
    \"result\": {\
        \"blueBtn\": 1,\
        \"redBtn\": 1\
    }\
}

[**注意事项**]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

[]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"} 

[需安装DobotLink才能连接并使用Dobot硬件设备
]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

[每台上位机有且只能运行一个DobotLink]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

[
]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

设备的端口（1-6）对应接口文档的端口号（0-5）

[
]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

 

**文档修订说明**

[
]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

 

+-----------+-----------+-----------+-----------+-----------+-----------+
| [         | [         | [版本]{   | [         | [修       | [备       |
| 序        | 时间]{sty | style="FO | 修订说    | 订人]{sty | 注]{style |
| 号]{style | le="FONT- | NT-SIZE:  | 明]{style | le="FONT- | ="FONT-SI |
| ="FONT-SI | SIZE: 10. | 10.       | ="FONT-SI | SIZE: 10. | ZE: 10.5p |
| ZE: 10.5p | 5pt; FONT | 5pt; FONT | ZE: 10.5p | 5pt; FONT | t; FONT-F |
| t; FONT-F | -FAMILY:  | -FAMILY:  | t; FONT-F | -FAMILY:  | AMILY: Ca |
| AMILY: Ca | Calibri;  | Calibri;  | AMILY: Ca | Calibri;  | libri; ms |
| libri; ms | mso-farea | mso-farea | libri; ms | mso-farea | o-fareast |
| o-fareast | st-font-f | st-font-f | o-fareast | st-font-f | -font-fam |
| -font-fam | amily: 宋 | amily: 宋 | -font-fam | amily: 宋 | ily: 宋体 |
| ily: 宋体 | 体; mso-b | 体; mso-b | ily: 宋体 | 体; mso-b | ; mso-bid |
| ; mso-bi  | idi-font- | idi-font- | ; mso-bi  | idi-font- | i-font-fa |
| di-font-f | family: ' | family: ' | di-font-f | family: ' | mily: 'Ti |
| amily: 'T | Times New | Times New | amily: 'T | Times New | mes New R |
| imes New  |  Roman';  |  Roman';  | imes New  |  Roman';  | oman'; ms |
| Roman'; m | mso-font- | mso-font- | Roman'; m | mso-font- | o-font-ke |
| so-font-k | kerning:  | kerning:  | so-font-k | kerning:  | rning: 1. |
| erning: 1 | 1.0000pt" | 1.0000pt" | erning: 1 | 1.0000pt" | 0000pt"}[ |
| .0000pt"} | }[]{style | }[]{style | .0000pt"} | }[]{style | ]{style   |
| []{       | ="FONT-SI | ="FONT-SI | []{style  | ="FONT-SI | ="FONT-SI |
| style="FO | ZE: 10.5p | ZE: 10.5p | ="FONT-SI | ZE: 10.5p | ZE: 10.5p |
| NT-SIZE:  | t; FONT-F | t; FONT-F | ZE: 10.5p | t; FONT-F | t; FONT-F |
| 10.5p     | AMILY: Ca | AMILY: Ca | t; FONT-F | AMILY: Ca | AMILY: Ca |
| t; FONT-F | libri; ms | libri; ms | AMILY: Ca | libri; ms | libri; ms |
| AMILY: Ca | o-fareast | o-fareast | libri; ms | o-fareast | o-fareast |
| libri; ms | -font-fam | -font-fam | o-fareast | -font-fam | -font-fam |
| o-fareast | ily: 宋体 | ily: 宋体 | -font-fam | ily: 宋体 | ily: 宋体 |
| -font-fam | ; mso-bi  | ; mso-bi  | ily: 宋体 | ; mso-bi  | ; mso-bi  |
| ily: 宋体 | di-font-f | di-font-f | ; mso-bi  | di-font-f | di-font-f |
| ; mso-bi  | amily: 'T | amily: 'T | di-font-f | amily: 'T | amily: 'T |
| di-font-f | imes New  | imes New  | amily: 'T | imes New  | imes New  |
| amily: 'T | Roman'; m | Roman'; m | imes New  | Roman'; m | Roman'; m |
| imes New  | so-font-k | so-font-k | Roman'; m | so-font-k | so-font-k |
| Roman'; m | erning: 1 | erning: 1 | so-font-k | erning: 1 | erning: 1 |
| so-font-k | .0000pt"} | .0000pt"} | erning: 1 | .0000pt"} | .0000pt"} |
| erning: 1 |           |           | .0000pt"} |           |           |
| .0000pt"} |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| [1]{sty   | [2        | [V1.0     | [创建     | [liuyufei | []{style  |
| le="FONT- | 019.11.11 | .0]{style | 文档]{sty | ]{style=" | ="FONT-SI |
| SIZE: 10. | ]{style=" | ="FONT-SI | le="FONT- | FONT-SIZE | ZE: 10.5p |
| 5pt; FONT | FONT-SIZE | ZE: 10.5p | SIZE: 10. | : 10.5pt; | t; FONT-F |
| -FAMILY:  | : 10.5pt; | t; FONT-F | 5pt; FONT |  FONT-FAM | AMILY: Ca |
| Calibri;  |  FONT-FAM | AMILY: Ca | -FAMILY:  | ILY: 宋体 | libri; ms |
| mso-farea | ILY: 宋体 | libri; ms | Calibri;  | ; mso-bi  | o-fareast |
| st-font-f | ; mso-bi  | o-fareast | mso-farea | di-font-f | -font-fam |
| amily: 宋 | di-font-f | -font-fam | st-font-f | amily: 'T | ily: 宋体 |
| 体; mso-b | amily: 'T | ily: 宋体 | amily: 宋 | imes New  | ; mso-bi  |
| idi-font- | imes New  | ; mso-bi  | 体; mso-b | Roman'; m | di-font-f |
| family: ' | Roman'; m | di-font-f | idi-font- | so-font-k | amily: 'T |
| Times New | so-font-k | amily: 'T | family: ' | erning: 1 | imes New  |
|  Roman';  | erning: 1 | imes New  | Times New | .0000pt;  | Roman'; m |
| mso-font- | .0000pt;  | Roman'; m |  Roman';  | mso-ascii | so-font-k |
| kerning:  | mso-ascii | so-font-k | mso-font- | -font-fam | erning: 1 |
| 1.0000pt" | -font-fam | erning: 1 | kerning:  | ily: Cali | .0000pt"} |
| }[]{style | ily: Cali | .0000pt"} | 1.0000pt" | bri; mso- |           |
| ="FONT-SI | bri; mso- |           | }[]{style | hansi-fon |           |
| ZE: 10.5p | hansi-fon |           | ="FONT-SI | t-family: |           |
| t; FONT-F | t-family: |           | ZE: 10.5p |  Calibri" |           |
| AMILY: Ca |  Calibri" |           | t; FONT-F | }[]{style |           |
| libri; ms | }[]{style |           | AMILY: Ca | ="FONT-SI |           |
| o-fareast | ="FONT-SI |           | libri; ms | ZE: 10.5p |           |
| -font-fam | ZE: 10.5p |           | o-fareast | t; FONT-F |           |
| ily: 宋体 | t; FONT-F |           | -font-fam | AMILY: Ca |           |
| ; mso-bi  | AMILY: Ca |           | ily: 宋体 | libri; ms |           |
| di-font-f | libri; ms |           | ; mso-bi  | o-fareast |           |
| amily: 'T | o-fareast |           | di-font-f | -font-fam |           |
| imes New  | -font-fam |           | amily: 'T | ily: 宋体 |           |
| Roman'; m | ily: 宋体 |           | imes New  | ; mso-bi  |           |
| so-font-k | ; mso-bi  |           | Roman'; m | di-font-f |           |
| erning: 1 | di-font-f |           | so-font-k | amily: 'T |           |
| .0000pt"} | amily: 'T |           | erning: 1 | imes New  |           |
|           | imes New  |           | .0000pt"} | Roman'; m |           |
|           | Roman'; m |           |           | so-font-k |           |
|           | so-font-k |           |           | erning: 1 |           |
|           | erning: 1 |           |           | .0000pt"} |           |
|           | .0000pt"} |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| [2]{sty   | [         | [         | []{style  | [         | []{style  |
| le="FONT- | ]{style=" | ]{style   | ="FONT-SI | ]{style=" | ="FONT-SI |
| SIZE: 10. | FONT-SIZE | ="FONT-SI | ZE: 10.5p | FONT-SIZE | ZE: 10.5p |
| 5pt; FONT | : 10.5pt; | ZE: 10.5p | t; FONT-F | : 10.5pt; | t; FONT-F |
| -FAMILY:  |  FONT-FAM | t; FONT-F | AMILY: Ca |  FONT-FAM | AMILY: Ca |
| Calibri;  | ILY: 宋体 | AMILY: Ca | libri; ms | ILY: 宋体 | libri; ms |
| mso-farea | ; mso-bid | libri; ms | o-fareast | ; mso-bid | o-fareast |
| st-font-f | i-font-fa | o-fareast | -font-fam | i-font-fa | -font-fam |
| amily: 宋 | mily: 'Ti | -font-fam | ily: 宋体 | mily: 'Ti | ily: 宋体 |
| 体; mso-b | mes New R | ily: 宋体 | ; mso-bi  | mes New R | ; mso-bi  |
| idi-font- | oman'; ms | ; mso-bi  | di-font-f | oman'; ms | di-font-f |
| family: ' | o-font-ke | di-font-f | amily: 'T | o-font-ke | amily: 'T |
| Times New | rning: 1. | amily: 'T | imes New  | rning: 1. | imes New  |
|  Roman';  | 0000pt; m | imes New  | Roman'; m | 0000pt; m | Roman'; m |
| mso-font- | so-ascii- | Roman'; m | so-font-k | so-ascii- | so-font-k |
| kerning:  | font-fami | so-font-k | erning: 1 | font-fami | erning: 1 |
| 1.0000pt" | ly: Calib | erning: 1 | .0000pt"} | ly: Calib | .0000pt"} |
| }[]{style | ri; mso-h | .0000pt"} |           | ri; mso-h |           |
| ="FONT-SI | ansi-font |           |  修改文档 | ansi-font |           |
| ZE: 10.5p | -family:  | [V5.      |           | -family:  |           |
| t; FONT-F | Calibri"} | 43]{style |           | Calibri"} |           |
| AMILY: Ca |           | ="FONT-SI |           |           |           |
| libri; ms | 20        | ZE: 10.5p |           | Kenan Wu  |           |
| o-fareast | 21.12.07  | t; FONT-F |           |           |           |
| -font-fam |           | AMILY: Ca |           |           |           |
| ily: 宋体 |           | libri; ms |           |           |           |
| ; mso-bi  |           | o-fareast |           |           |           |
| di-font-f |           | -font-fam |           |           |           |
| amily: 'T |           | ily: 宋体 |           |           |           |
| imes New  |           | ; mso-bi  |           |           |           |
| Roman'; m |           | di-font-f |           |           |           |
| so-font-k |           | amily: 'T |           |           |           |
| erning: 1 |           | imes New  |           |           |           |
| .0000pt"} |           | Roman'; m |           |           |           |
|           |           | so-font-k |           |           |           |
|           |           | erning: 1 |           |           |           |
|           |           | .0000pt"} |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+

[]{style="FONT-SIZE: 10.5pt; FONT-FAMILY: 宋体; mso-spacerun: 'yes'; mso-bidi-font-family: 'Times New Roman'; mso-font-kerning: 1.0000pt; mso-ascii-font-family: Calibri; mso-hansi-font-family: Calibri"}

 

 

 

 

 
:::

::: {#winchm_template_footer}
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
:::
:::

\

------------------------------------------------------------------------

\
This file is decompiled from a .CHM file\
by an UNREGISTERED version of Easy CHM.\
You can download Easy CHM at :
[http://www.eTextWizard.com](http://www.etextwizard.com/){target="_blank"}\
\
