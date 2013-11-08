RS232 COM port native driver for 1C

This is RS232 communication port native driver for 1�:Enterprise 8.x.
This driver provides communication from 1�:Enterprise 8.x to lots of devices that use 
RS232 communication port, such as: modems, thermal printers, bar code scanners and special controllers.

Methods:
int Open(int nPort, int Baud, int nBit, int Parity, int ) � open port, return 0 if success;
Close() � close port;
int Send(wstr data) � send data;
int Receive() � receive data from port � return number of received chars; 
Delay(int dt) � delay dt milliseconds.

Properties
bool IsOpen � is port opened or no;
int Port � port number;
int Baud � port speed;
int ByteSize � number of bits;
int Parity � port parity;
int StopBit" � 1, 1,5 2 stop bit;
wstr Command � last command to port;
wstr Answer � answer from port;
int Error � last error code

