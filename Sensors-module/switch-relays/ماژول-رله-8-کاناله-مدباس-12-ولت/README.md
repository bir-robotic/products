##8 Channel

1.Description:
It is a 8-Channels ModbusRTU relay module equipped with mature and stable 8-bit MCU and RS485 level communication chip,adopt standard MODBUS RTU format RS485 communication protocol. It can realize 8bit input signal detection and 8bit relay output. It can be used for digital detection or power control occasions..

2.Features:
1>.Support Modbus RTU protocol
2>.Support RS485/TTL UART interface
3>.Output indicator in multi mode
4>.Address can be set
5>.Support input reverse connection protection
6>.Relay switch output
7>.Support parameter memory function
8>.Optocoupler isolation

3.Parameters:
1>.Product name: 8Bit MODBUS RTU Relay Module
3>.Work voltage:DC 12V
3>.Work current:1A
4>.Baud rate:4800/9600/19600bps(default 9600bps)
5>.Optocoupler input signal:DC 12V
6>.Set address:1~255
7>.Relay control mode: ON/OFF,Delay_ON,Delay_OFF mode
8>.Delay time: 0~25.5s 
9>.Load: AC 250V 10A or DC 30V 10A
10>.Protocol:Modbus RTU
11>.Interface:RS485/TTL UART
12>.Control channel: 8channel
13>.Work Temperature:-20℃~85℃
14>.Work Humidity:10%~85%RH
15>.PCB Size:145*78*22mm

4.MODBUS RTU Command:
1>.Baud rate: 9600,8,None,1
/****************Set Device Address**************************************************/
2>.Set device address to 0x01: 00 10 00 00 00 01 02 00 01 6A 00
3>.Set device address to 0x02: 00 10 00 00 00 01 02 00 02 2A 01
4>.Set device address to 0x03: 00 10 00 00 00 01 02 00 03 EB C1
/****************Command Format****************************************************/
5>.Read device address: 00 03 00 00 00 01 85 db
Return:00 03 02 00 01 44 44 //01 is device address.
6>.Set command format: 
Turn ON 1# relay: 01 05 00 01 01 00 9d 9a
Note_1:The 1st byte is device address.
Note_2:The 2nd byte is function code.
Note_3:The 3rd and 4th byte are relay/register addresses. So it can be 0x0000, 0x0001, 0x0002, 0x0003, 0x0004, 0x0005, 0x0006, 0x0007.
Note_4:The 5th and 6th byte are relay/register data. 01 means turn ON relay and 00 means turn OFF relay.
Note_5:The 7th and 8th byte are CRC code.
/****************Turn ON/OFF Relay*************************************************/
7>.Turn ON 0# relay: 01 05 00 00 FF 00 8C 3A
Turn OFF 0# relay: 01 05 00 00 00 00 CD CA
8>.Turn ON 1# relay: 01 05 00 01 FF 00 DD FA
Turn OFF 1# relay: 01 05 00 01 00 00 9C 0A
9>.Turn ON 2# relay: 01 05 00 02 FF 00 2D FA
Turn OFF 2# relay: 01 05 00 02 00 00 6C 0A
10>.Turn ON 3# relay: 01 05 00 03 FF 00 7C 3A
Turn OFF 3# relay: 01 05 00 03 00 00 3D CA
11>.Turn ON 4# relay: 01 05 00 04 FF 00 CD FB
Turn OFF 4# relay: 01 05 00 04 00 00 8C 0B
12>.Turn ON 5# relay: 01 05 00 05 FF 00 9C 3B
Turn OFF 5# relay: 01 05 00 05 00 00 DD CB
13>.Turn ON 6# relay: 01 05 00 06 FF 00 6C 3B
Turn OFF 6# relay: 01 05 00 06 00 00 2D CB
14>.Turn ON 7# relay: 01 05 00 07 FF 00 3D FB
Turn OFF 7# relay: 01 05 00 07 00 00 7C 0B
/****************Read Relay Status***************************************************/
15>.Read 0# relay status: 01 01 00 00 00 01 FD CA
16>.Read 1# relay status: 01 01 00 01 00 01 AC 0A
17>.Read 2# relay status: 01 01 00 02 00 01 5C 0A
18>.Read 3# relay status: 01 01 00 03 00 01 0D CA
19>.Read 4# relay status: 01 01 00 04 00 01 BC 0B
20>.Read 5# relay status: 01 01 00 05 00 01 ED CB
21>.Read 6# relay status: 01 01 00 06 00 01 1D CB
23>.Read 7# relay status: 01 01 00 07 00 01 4C 0B
24>.Read all relay status: 01 01 00 00 00 08 3D CC
/****************Turn ON Delay Mode************************************************/
25>.Function: Relay will turn ON for a delay time and then turn OFF.
26>.The unit of delay time is 100ms[It means 1 is 100ms]
27>.Control 1# device 0# relay: 01 05 02 00 07 00 CE 42 //7*100ms = 700ms
28>.Control 1# device 1# relay: 01 05 02 01 08 00 9A 72  //800MS
29>.Control 2# device 0# relay: 02 05 02 00 05 00 CF 11  //500MS
30>.Control 2# device 1# relay: 02 05 02 01 06 00 9E 21  //600MS
31>.Turn ON all relay: 01 0F 00 00 00 08 01 00 FE 95
32>.Turn ON all relay: 01 0F 00 00 00 08 01 FF BE D5
/****************Reverse Output State************************************************/
33>.Reverse 0# relay: 01 05 00 00 55 00 F2 9A
34>.Reverse 1# relay: 01 05 00 01 55 00 A3 5A
35>.Reverse 2# relay: 01 05 00 02 55 00 53 5A
36>.Reverse 3# relay: 01 05 00 03 55 00 02 9A
37>.Reverse 4# relay: 01 05 00 04 55 00 B3 5B
38>.Reverse 5# relay: 01 05 00 05 55 00 E2 9B
49>.Reverse 6# relay: 01 05 00 06 55 00 12 9B
40>.Reverse 7# relay: 01 05 00 07 55 00 43 5B
41>.Reverse all relay: 01 05 00 00 5A 00 F7 6A
/****************Read 8-Bit Input State***********************************************/
42>.Send: 01 02 00 00 00 08 79 CC
43>.Receive:01 02 01 00 A1 88

5.Application:
1>.Embedded system control
2>.Industrial control
3>.Micro mobile device control

6.Package:
1>.1pc 8-Bit MODBUS RTU Relay Module

<h1 align="center">
  <img src="https://raw.githubusercontent.com/bir-robotic/products/main/Sensors-module/switch-relays/%D9%85%D8%A7%DA%98%D9%88%D9%84-%D8%B1%D9%84%D9%87-8-%DA%A9%D8%A7%D9%86%D8%A7%D9%84%D9%87-%D9%85%D8%AF%D8%A8%D8%A7%D8%B3-12-%D9%88%D9%84%D8%AA/Hd53ca047f1c746e79172480a57b08540D.webp" alt="8 Channel" width="700px">
  <br>
</h1>
<h1 align="center">
  <img src="https://raw.githubusercontent.com/bir-robotic/products/main/Sensors-module/switch-relays/%D9%85%D8%A7%DA%98%D9%88%D9%84-%D8%B1%D9%84%D9%87-8-%DA%A9%D8%A7%D9%86%D8%A7%D9%84%D9%87-%D9%85%D8%AF%D8%A8%D8%A7%D8%B3-12-%D9%88%D9%84%D8%AA/Hf2226ab221954c73bac1008708a3f0fe5.webp" alt="8 Channel" width="700px">
  <br>
</h1>
<h1 align="center">
  <img src="https://raw.githubusercontent.com/bir-robotic/products/main/Sensors-module/switch-relays/%D9%85%D8%A7%DA%98%D9%88%D9%84-%D8%B1%D9%84%D9%87-8-%DA%A9%D8%A7%D9%86%D8%A7%D9%84%D9%87-%D9%85%D8%AF%D8%A8%D8%A7%D8%B3-12-%D9%88%D9%84%D8%AA/H26625b0f389e447fb74cff4d640605e81.webp" alt="8 Channel" width="700px">
  <br>
</h1>
<h1 align="center">
  <img src="https://raw.githubusercontent.com/bir-robotic/products/main/Sensors-module/switch-relays/%D9%85%D8%A7%DA%98%D9%88%D9%84-%D8%B1%D9%84%D9%87-8-%DA%A9%D8%A7%D9%86%D8%A7%D9%84%D9%87-%D9%85%D8%AF%D8%A8%D8%A7%D8%B3-12-%D9%88%D9%84%D8%AA/H9b567056115e449480e70241d79f61e97.webp" alt="8 Channel" width="700px">
  <br>
</h1>
<h1 align="center">
  <img src="https://raw.githubusercontent.com/bir-robotic/products/main/Sensors-module/switch-relays/%D9%85%D8%A7%DA%98%D9%88%D9%84-%D8%B1%D9%84%D9%87-8-%DA%A9%D8%A7%D9%86%D8%A7%D9%84%D9%87-%D9%85%D8%AF%D8%A8%D8%A7%D8%B3-12-%D9%88%D9%84%D8%AA/H492919921b8b4d609ff7a5151b4fcb6ep.webp" alt="8 Channel" width="700px">
  <br>
</h1>
<h1 align="center">
  <img src="https://raw.githubusercontent.com/bir-robotic/products/main/Sensors-module/switch-relays/%D9%85%D8%A7%DA%98%D9%88%D9%84-%D8%B1%D9%84%D9%87-8-%DA%A9%D8%A7%D9%86%D8%A7%D9%84%D9%87-%D9%85%D8%AF%D8%A8%D8%A7%D8%B3-12-%D9%88%D9%84%D8%AA/H3e0af0686def48b884545cda2bf7f6dbV.webp" alt="8 Channel" width="700px">
  <br>
</h1>
