# Modbus与总线寄存器

### ModbusCreate
ModbusCreate
- **原型**：
ModbusCreate(ip,port,slave_id,isRTU)
- **描述**：
创建Modbus主站，并和从站建立连接。最多支持同时连接5个设备。
- **必选参数**：
ip
port
slave_id
- **可选参数**：
参数名
类型
说明
string
int
int
从站IP地址。
从站端口。
从站ID。
参数名
类型
说明
isRTU
int
如果不携带或为0，建立modbusTCP通信。 如果为1，建立
modbusRTU通信。
注意：
此参数决定了连接建立后传输数据使用的协议格式，并不影响连接结果。因此，如果创建主
站时该参数设置错误，依然可以创建成功，但后续通讯时会导致异常。
- **返回**：
ErrorID,{index},ModbusCreate(ip,port,slave_id,isRTU);
ErrorID为0表示创建成功，-1表示创建失败，其余错误码请参考通用错误码
index为返回的主站索引，后续调用其他Modbus指令时使用
- **示例**：ModbusCreate("127.0.0.1",60000,1,0)
建立modbusTCP通信主站，连接本机的Modbus从站，端口为60000，从站ID为1。

---

### ModbusRTUCreate
ModbusRTUCreate
- **原型**：ModbusRTUCreate(slave_id,baud,parity,data_bit,stop_bit)
- **描述**：创建基于RS485接口的Modbus主站，并和从站建立连接。最多支持同时连接5个设备。
- **必选参数**：
参数名
类型
说明
slave_id
baud
- **可选参数**：
int
int
从站ID。
RS485接口的波特率。
参数名
类型
说明
parity
string
是否有奇偶校验位。"O"表示奇校验，"E"表示偶校验，"N"表示无奇
偶校验位。默认值为“E”。
data_bit
stop_bit
int
int
数据位长度。默认值为8。
停止位长度。默认值为1。
- **返回**：ErrorID,{index},ModbusRTUCreate(slave_id,baud,parity,data_bit,stop_bit);
ErrorID为0表示创建成功，-1表示创建失败，其余错误码请参考通用错误码
index为返回的主站索引，后续调用其他Modbus指令时使用
- **示例**：ModbusRTUCreate(1,115200)
创建Modbus主站并与RS485接口连接的从站建立连接，从站ID为1，波特率为115200。

---

### ModbusClose
ModbusClose
- **原型**：
ModbusClose(index)
- **描述**：
和Modbus从站断开连接，释放主站。
- **必选参数**：
参数名
类型
说明
index
int
创建主站时返回的主站索引。
- **返回**：
ErrorID,{},ModbusClose(index);
- **示例**：ModbusClose(0)
释放索引为0的Modbus主站。

---

### GetInBits
GetInBits
- **原型**：
GetInBits(index,addr,count)
- **描述**：
读取Modbus从站触点寄存器（离散输入）地址的值。
- **必选参数**：
参数名
类型
说明
int
int
int
index
addr
count
- **返回**：
创建主站时返回的主站索引。
触点寄存器起始地址。
连续读取触点寄存器的值的数量。取值范围：[1, 16]。
ErrorID,{value1,value2,...,valuen},GetInBits(index,addr,count);
{value1,value2,...,valuen}为读取的值，数量与count相同。
- **示例**：GetInBits(0,3000,5)
从地址为3000的触点寄存器开始读取5个值。

---

### GetInRegs
GetInRegs
- **原型**：
GetInRegs(index,addr,count,valType)
- **描述**：
按照指定的数据类型，读取Modbus从站输入寄存器地址的值。
- **必选参数**：
参数名
类型
说明
int
int
int
index
addr
count
- **可选参数**：
创建主站时返回的主站索引。
输入寄存器起始地址。
连续读取输入寄存器的值的数量。取值范围：[1, 4]。
参数名
类型
说明
读取的数据格式：
U16：16位无符号整数（2个字节，占用1个寄存器）；
U32：32位无符号整数（4个字节，占用2个寄存器）；
F32：32位单精度浮点数（4个字节，占用2个寄存器）；
F64：64位双精度浮点数（8个字节，占用4个寄存器）；
默认值为U16。
valType
string
- **返回**：
ErrorID,{value1,value2,...,valuen},GetInRegs(index,addr,count,valType);
{value1,value2,...,valuen}为读取的值，数量与count相同。
- **示例**：GetInRegs(0,4000,3)
从地址为4000的输入寄存器开始读取3个值，值类型为U16。

---

### GetCoils
GetCoils
- **原型**：
GetCoils(index,addr,count)
- **描述**：
读取Modbus从站线圈寄存器地址的值。
- **必选参数**：
参数名
类型
说明
int
int
int
index
addr
count
- **返回**：
创建主站时返回的主站索引。
线圈寄存器起始地址。
连续读取线圈寄存器的值的数量。取值范围：[1, 16]。
ErrorID,{value1,value2,...,valuen},GetCoils(index,addr,count);
{value1,value2,...,valuen}为读取的值，数量与count相同。
- **示例**：GetCoils(0,1000,3)
从地址为1000的线圈寄存器开始读取3个值。

---

### SetCoils
SetCoils
- **原型**：
SetCoils(index,addr,count,valTab)
- **描述**：
将指定的值写入线圈寄存器指定的地址。
- **必选参数**：
参数名
类型
说明
index
addr
count
int
int
int
创建主站时返回的主站索引。
线圈寄存器起始地址。
连续写入线圈寄存器的值的数量。取值范围：[1, 16]。
valTab
string
要写入的值，数量与count相同。
- **返回**：
ErrorID,{},SetCoils(index,addr,count,valTab);
- **示例**：SetCoils(0,1000,3,{1,0,1})
从地址为1000的线圈寄存器开始连续写入3个值，分别为1，0，1。

---

### GetHoldRegs
GetHoldRegs
- **原型**：
GetHoldRegs(index,addr,count,valType)
- **描述**：
按照指定的数据类型，读取Modbus从站保持寄存器地址的值。
- **必选参数**：
参数名
类型
说明
index
addr
count
int
int
int
- **可选参数**：
创建主站时返回的主站索引，最多支持5个设备。取值范围：[0,4]。
保持寄存器起始地址。
连续读取保持寄存器的值的数量。
参数名
类型
说明
读取的数据类型：
U16：16位无符号整数（2个字节，占用1个寄存器）；
U32：32位无符号整数（4个字节，占用2个寄存器）；
F32：32位单精度浮点数（4个字节，占用2个寄存器）；
F64：64位双精度浮点数（8个字节，占用4个寄存器）；
默认值为U16。
valType
string
- **返回**：
ErrorID,{value1,value2,...,valuen},GetHoldRegs(index,addr,count,valType);
{value1,value2,...,valuen}为读取的值，数量与count相同。
- **示例**：GetHoldRegs(0,3095,1)
从地址为3095的保持寄存器开始读取1个值，值类型为U16。

---

### SetHoldRegs
SetHoldRegs
- **原型**：
SetHoldRegs(index,addr,count,valTab,valType)
- **描述**：
将指定的值以指定的数据类型写入Modbus从站保持寄存器指定的地址。
- **必选参数**：
参数名
类型
说明
index
addr
count
int
int
int
创建主站时返回的主站索引，最多支持5个设备。取值范围：[0,4]。
保持寄存器起始地址。
连续写入保持寄存器的值的数量。取值范围：[1, 4]
valTab
string
要写入的值，数量与count相同。
- **可选参数**：
参数名
类型
说明
写入的数据类型：
U16：16位无符号整数（2个字节，占用1个寄存器）；
U32：32位无符号整数（4个字节，占用2个寄存器）；
F32：32位单精度浮点数（4个字节，占用2个寄存器）；
F64：64位双精度浮点数（8个字节，占用4个寄存器）；
默认值为U16。
valType
string
- **返回**：
ErrorID,{},SetHoldRegs(index,addr,count,valTab,valType);
- **示例**：SetHoldRegs(0,3095,2,{6000,300}, U16)
从地址为3095的保持寄存器开始写入两个U16类型的值，分别为6000和300。
2.6 总线寄存器相关指令
指令列表
总线寄存器指令用于读写Profinet或Ethernet/IP总线寄存器。
指令
功能
指令类型
GetInputBool
获取输⼊寄存器指定地址的bool值
GetInputInt
获取输⼊寄存器指定地址的int值
GetInputFloat
获取输⼊寄存器指定地址的float值
GetOutputBool
获取输出寄存器指定地址的bool值
GetOutputInt
获取输出寄存器指定地址的int值
GetOutputFloat
获取输出寄存器指定地址的float值
SetOutputBool
设置输出寄存器指定地址的bool值
SetOutputInt
设置输出寄存器指定地址的int值
SetOutputFloat
设置输出寄存器指定地址的float值
立即指令
立即指令
立即指令
立即指令
立即指令
立即指令
立即指令
立即指令
立即指令

---

### GetInputBool
GetInputBool
- **原型**：GetInputBool(address)
- **描述**：获取输⼊寄存器指定地址的bool类型的数值。
- **必选参数**：
参数名
类型
说明
address
int
寄存器地址，取值范围：[0,63]。
- **返回**：
ErrorID,{value},GetInputBool(address);
value表示指定的寄存器地址的值，为0或1。
- **示例**：GetInputBool(0)
读取输入寄存器地址位0的布尔值。

---

### GetInputInt
GetInputInt
- **原型**：GetInputInt(address)
- **描述**：获取输⼊寄存器指定地址的int类型的数值。
- **必选参数**：
参数名
类型
说明
address
int
寄存器地址，取值范围：[0,23]。
- **返回**：
ErrorID,{value},GetInputInt(address);
value表示指定的寄存器地址的值，为整型数（int32）。
- **示例**：GetInputInt(1)
读取输入寄存器地址位1的int值。

---

### GetInputFloat
GetInputFloat
- **原型**：GetInputFloat(address)
- **描述**：获取输⼊寄存器指定地址的float类型的数值。
- **必选参数**：
参数名
类型
说明
address
int
寄存器地址，取值范围：[0,23]。
- **返回**：
ErrorID,{value},GetInputFloat(address);
value表示指定的寄存器地址的值，为单精度浮点数（float）
- **示例**：GetInputFloat(2)
读取输入寄存器地址位2的float值。

---

### GetOutputBool
GetOutputBool
- **原型**：GetOutputBool(address)
- **描述**：获取输出寄存器指定地址的bool类型的数值。
- **必选参数**：
参数名
类型
说明
address
int
寄存器地址，取值范围：[0,63]。
- **返回**：
ErrorID,{value},GetOutputBool(address);
value表示指定的寄存器地址的值，为0或1。
- **示例**：GetOutputBool(0)
获取输出寄存器地址位0的布尔值。

---

### GetOutputInt
GetOutputInt
- **原型**：GetOutputInt(address)
- **描述**：获取输出寄存器指定地址的int类型的数值。
- **必选参数**：
参数名
类型
说明
address
int
寄存器地址，取值范围：[0,23]。
- **返回**：
ErrorID,{value},GetOutputInt(address);
value表示指定的寄存器地址的值，为整型数（int32）。
- **示例**：GetOutputInt(1)
读取输出寄存器地址位1的int值。

---

### GetOutputFloat
GetOutputFloat
- **原型**：GetOutputFloat(address)
- **描述**：获取输出寄存器指定地址的float类型的数值。
- **必选参数**：
参数名
类型
说明
address
int
寄存器地址，取值范围：[0,23]。
- **返回**：
ErrorID,{value},GetOutputFloat(address);
value表示指定的寄存器地址的值，为单精度浮点数（float）。
- **示例**：GetOutputFloat(2)
读取输出寄存器地址位2的float值。

---

### SetOutputBool
SetOutputBool
- **原型**：SetOutputBool(address,value)
- **描述**：设置输出寄存器指定地址的bool类型的数值。
- **必选参数**：
参数名
类型
说明
address
value
- **返回**：
int
int
寄存器地址，取值范围：[0,63]。
要设置的值，支持0或1。
ErrorID,{},SetOutputBool(address, value);
- **示例**：SetOutputBool(0,0)
设置输出寄存器0的值为假。

---

### SetOutputInt
SetOutputInt
- **原型**：SetOutputInt(address,value)
- **描述**：设置输出寄存器指定地址的int类型的数值。
- **必选参数**：
参数名
类型
说明
address
value
- **返回**：
int
int
寄存器地址，取值范围：[0,23]。
要设置的值，支持带符号的32位整型数。
ErrorID,{},SetOutputInt(address,value);
- **示例**：SetOutputInt(1,123)
设置输出寄存器地址位1的值为123。

---

### SetOutputFloat
SetOutputFloat
- **原型**：SetOutputFloat(address,value)
- **描述**：设置输出寄存器指定地址的float类型的数值。
- **必选参数**：
参数名
类型
说明
address
value
- **返回**：
int
float
寄存器地址，取值范围：[0,23]。
要设置的值，支持单精度浮点数。
ErrorID,{},SetOutputFloat(address,value);
- **示例**：SetOutputFloat(2,12.3)
设置输出寄存器地址位2的float值为12.3。

---

